---
category: Treatment
path: '/treatment'
title: 'GET treatments for a patient'
type: 'GET'

layout: nil
---

Returns a list of treatments associated with a patient

### Path
```GET /patient/:patient_id/treatments/ ```

### Parameters
```id: integer - Patient id ```

### Response Example
```[
  {
    "id" : 1001
    "medication" : {
      "id" : 1001
      "name" : "HEPARIN SODIUM"
    },
    "dosage" : "100mL / hour",
    "start_date" : "2019-04-01T00:00:00Z",
    "end_date" : null
  },
  {
    "id" : 1000
    "medication" : {
      "id" : 1002
      "name" : "Naproxen Sodium"
    },
    "dosage" : "1000IU / day",
    "start_date" : "2017-01-01T00:00:00Z",
    "end_date" : "2018-12-31T00:00:00Z"
  }
]```

