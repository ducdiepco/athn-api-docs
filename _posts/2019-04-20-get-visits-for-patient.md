---
category: Visit
path: '/visit'
title: 'GET visits for a patient'
type: 'GET'

layout: nil
---

Returns a list of visits associated with a patient

### Path
```GET /patient/:patient_id/visits/ ```

### Parameters
```id: integer - Patient id ```

### Response Example
```[
  {
    "id" : 1001
      "provider" : {
        "id" : 1002,
          "first_name" : "Robena",
          "last_name" :	"Dillet",
          "office_address" : "3241 Montana Parkway",
          "office_city" : "Fayetteville",
          "office_state" :	"North Carolina"
      },
      "visit_date" : "2017-01-01T00:00:00Z",
      "notes" : "I saw this patient"
  }
]```
