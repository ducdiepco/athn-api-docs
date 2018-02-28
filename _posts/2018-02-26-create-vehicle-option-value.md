---
category: Mutations
path: '/Mutations'
title: 'Create Vehicle Option Value'
type: 'MUTATION'

layout: nil
---

Create a new vehicle option value

### Operation name
```createVehicleOptionValue ```

### Fields

```name: String - Name for vehicle option value ```
```description: String - description for vehicle option value```
```vehicle_option_type_id: Integer - Vehicle Option Type Id```

### Query Example

```mutation createVehicleOptionValue {
  createVehicleOptionValue(
    name: "S 4dr Sedan (2.5L 4cyl 6A)",
    description: "option value description",
    vehicle_option_type_id: 4
  ) {
    id
    name
    description
    vehicle_option_type {
      id
      name
    }
  }
}```

### Response Example
```{
  "data": {
    "createVehicleOptionValue": {
      "id": 7,
      "name": "S 4dr Sedan (2.5L 4cyl 6A)",
      "description": "option value description",
      "vehicle_option_type": {
        "id": 4,
        "name": "trim"
      }
    }
  }
}```
