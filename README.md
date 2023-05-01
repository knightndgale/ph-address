# Data Deconstruct Addresses

This repository contains data for deconstructing Philippine addresses into 
their component parts, including region, province, municipality/city, and 
barangay. The components are connected via `regCode`, `provCode`, and 
`citymunCode`, with the barangay being connected to the stream of 
`idcode`.

## Data Structure

The data is structured as follows:

### Region

```js
{
id: 1,
psgcCode: "010000000",
regDesc: "REGION I (ILOCOS REGION)",
regCode: "01",
},
```

### Province

```js
{
id: 88,
psgcCode: "168500000",
provDesc: "DINAGAT ISLANDS",
regCode: "16",
provCode: "1685",
},
```

### Municipality/City


```js
{
id: 1647,
psgcCode: "168507000",
citymunDesc: "TUBAJON",
regDesc: "16",
provCode: "1685",
citymunCode: "168507",
},
```

### Barangay


```js
{
id: 42029,
brgyCode: "168507009",
brgyDesc: "Santa Cruz (Pob.)",
regCode: "16",
provCode: "1685",
citymunCode: "168507",
},
```


## Notes for Users

- The `region` data includes the `id`, `psgcCode`, `regDesc`, and 
`regCode`.
- The `province` data includes the `id`, `psgcCode`, `provDesc`, 
`regCode`, and `provCode`.
- The `municipality/city` data includes the `id`, `psgcCode`, 
`citymunDesc`, `regCode`, `provCode`, and `citymunCode`.
- The `barangay` data includes the `id`, `brgyCode`, `brgyDesc`, 
`regCode`, `provCode`, and `citymunCode`.
- The components are connected via `regCode`, `provCode`, and 
`citymunCode`, with the barangay being connected to the stream of 
`idcode`.

