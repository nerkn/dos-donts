# Go Golang
It seems they dont care about structure of program, it looks like messy if programmer dont specially take care

Making json out of db query is very primitive, no destructiring, 

Cat is struct;

    func getCats(db  *sql.DB ) []Cat{
      cats := make([]Cat, 0)
      rows, err := db.Query("select id, name, cid, parent from 03cats limit 100")
      if(err != nil ){
        panic(err)
      }

      for rows.Next() {
        tempcat := Cat{0,"",0,0}
        if err := rows.Scan(&tempcat.Id, &tempcat.Name, &tempcat.Cid, &tempcat.Parent); err != nil {
          panic(err)
        }
        //fmt.Println(tempcat)
        cats = append(cats, tempcat)
      }
      return cats;
      }
    

  
