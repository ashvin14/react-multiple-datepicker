# React Multiple Datepicker 📅

[![](https://raw.githubusercontent.com/codeinfuse/react-multiple-datepicker/master/demo/react-multiple-datepicker-screenshot.png)](https://codesandbox.io/s/p7q599zlqq)

Let's the user pick more than one date from the date picker.

## Motivation

After looking at various date picking libraries out there I couldn't find a single one who lets users pick more than one date without enforcing a range, so I decided to write one myself.

## installation

```
npm install react-multiple-datepicker --save

```

OR

```
yarn add react-multiple-datepicker

```
## Usage


```javascript
import MultipleDatePicker from 'react-multiple-datepicker'


render() {
  <MultipleDatePicker
    onSubmit={dates => console.log('selected date', dates)}
  />
}
```
## Api
### props
* onSubmit

   A callback function which has selected dates from Component as Argument
 

* selectedDatesArray
   
   takes array of dates ,and prefills the component with those dates.
   ```javascript
   import MultipleDatePicker from "react-multiple-datepicker"

   render(){
    <MultipleDatePicker
        selectedDatesArray={[new Date("2018-10-01"),new Date("2018-10-07")]}
    />
   }
   ```




## Roadmap

* [ ] Make it responsive
* [ ] Support for `onDateSelect` prop.
* [ ] Add test cases

## Note From Author

Hi, thanks for checking out this library. You can read more about me at https://bilalbudhani.com/about or you can follow me at https://twitter.com/BilalBudhani

