---
category: Diagnosis
path: '/diagnosis'
title: 'GET diagnoses for a patient'
type: 'GET'

layout: nil
---

Returns a list of diagnoses associated with a patient

### Path
```GET /patient/:patient_id/diagnoses/ ```

### Parameters
```id: integer - Patient id ```

### Response Example
```[
  {
    "id" : 1001
      "diagnosis" : {
        "id" : 1001
          "name" : "Kernicterus due to isoimmunization"
      },
      "diagnosing_provider" : {
        "id" : 1002,
        "first_name" : "Robena",
        "last_name" : "Dillet",
        "office_address" : "3241 Montana Parkway",
        "office_city" : "Fayetteville",
        "office_state" : "North Carolina"
      },
      "start_date" : "2017-01-01T00:00:00Z",
      "end_date" : "2018-12-31T00:00:00Z"
  }
]```
