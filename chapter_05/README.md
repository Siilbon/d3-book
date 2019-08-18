# Data
This chapter talks about loading data and using it to manipulate the DOM.

## Notes
- The 'then' function is used to assure that the data has been loaded (callback function)

```javascript
d3.csv("food.csv", function(d) {
  return {
    Food: d.Food
    Deliciousness: parseFloat(d.Deliciousness)
  };
}).then(function(data) {
  console.log(data);
});
```
- The style can be manipulated using condidtional formatting