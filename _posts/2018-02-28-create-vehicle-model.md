---
category: Mutations
path: '/Mutations'
title: 'Create Vehicle Model'
type: 'MUTATION'

layout: nil
---

Create a new vehicle model

### Operation name
```createVehicleModel ```

### Arguments

```description_cont: String - Search by description```
```name_cont: String - Search by name```

### Query Example

``` query {
  searchVehicleModels(filter: {name_cont: "Fusion"} ) {
    id
    name
    description
    vehicle_make{
      name
    }
    vehicle{
      name
    }
    vehicle_option_types {
      id
      name
      vehicle_option_values {
        id
        name
      }
    }
  }
}
```

### Response Example

```{
  "data": {
    "searchVehicleModels": [
      {
        "id": 9,
        "name": "Fusion",
        "description": "Ford Fusion",
        "vehicle_make": {
          "name": "Ford"
        },
        "vehicle": {
          "name": "Sedan"
        },
        "vehicle_option_types": [
          {
            "id": 1,
            "name": "trim",
            "vehicle_option_values": [
              {
                "id": 1,
                "name": "S 4dr Sedan (2.5L 4cyl 6A)"
              },
              {
                "id": 2,
                "name": "SE 4dr Sedan AWD w/EcoBoost (2.0L 4cyl Turbo 6M)"
              }
            ]
          }
        ]
      }
    ]
  }
} ```
