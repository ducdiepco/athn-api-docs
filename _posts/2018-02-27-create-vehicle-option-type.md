---
category: Mutations
path: '/Mutations'
title: 'Create Vehicle Option Type'
type: 'MUTATION'

layout: nil
---

Create a new vehicle option type

### Operation name
```createVehicleOptionType ```

### Fields

```name: String - Name for option type ```
```description: String - description for option type```

### Query Example

```mutation createVehicleOptionType {
  createVehicleOptionType(
    name: "trim",
    description: "Trim Description",
  ) {
    id
    name
    description
  }
}```

### Response Example
```{
  "data": {
    "createVehicleOptionType": {
      "id": 4,
      "name": "trim",
      "description": "Trim Description"
    }
  }
}```
