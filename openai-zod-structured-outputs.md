Currently openAi hid specification under well known wonderful library called Zod. While my existing application dont need this unnecessary dependency, I want to use bare definition that it produces. I'm almost sure openai not only conforms this but any format provided but I specially want to know what zod produces

```json

const CalendarEvent = z.object({
  name: z.string(),
  date: z.string(),
  participants: z.array(z.string()),
});

let request =  JSON.stringify( zodResponseFormat(CalendarEvent, "event"), null, 2);
```

this is transformed into 

```json

 {
   "type": "json_schema",
   "json_schema": {
     "name": "event",
     "strict": true,
     "schema": {
       "type": "object",
       "properties": {
         "name": {
           "type": "string"
         },
         "date": {
           "type": "string"
         },
         "participants": {
           "type": "array",
           "items": {
             "type": "string"
           }
         }
       },
       "required": [
         "name",
         "date",
         "participants"
       ],
       "additionalProperties": false,
       "$schema": "http://json-schema.org/draft-07/schema#"
     }
   }
}
```
