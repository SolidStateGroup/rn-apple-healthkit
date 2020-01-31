Get the most recent BMI sample.

On success, the callback function will be provided with a `waist` object containing the waist `value`, and the `startDate` and `endDate` of the sample. *Note: startDate and endDate will be the same as waist samples are saved at a specific point in time.*

```javascript
let options = {
  unit: 'inch'
};
```

```javascript
AppleHealthKit.getLatestWaistCircumference(options, (err: string, results: Object) => {
    if (err) {
        console.log("error getting latest waist data: ", err);
        return;
    }
    console.log(results)
});
```

```javascript
{
	value: 76.2,
	startDate: '2016-07-08T12:00:00.000-0400',
	endDate: '2016-07-08T12:00:00.000-0400'
}
```
