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
        selectedDatesArray={[new Date("2018-10-01"),new Date("2018-10-07")]} />
   }
   ```

* minDate
    renders the calender from specified minDate .accepts date value for prop.

    ```javascript
    import MultipleDatePicker from "react-multiple-datepicker";

    render(){
        <MultipleDatePicker 
        minDate={new Date("2018-07-17")} />
    }
    ```

* maxDate
    renders the calender till specified maxDate .accepts date value for prop.

    ```javascript
    import MultipleDatePicker from "react-multiple-datepicker";

    render(){
        <MultipleDatePicker 
        maxDate={new Date("2018-07-17")} />
    }
    ```

### Child Components
 you can add child Components , and it will render the child Components which when clicked on opens calendar Component.By default it renders input text.

```javascript
    import MultipleDatePicker from "react-multiple-datepicker";

    render(){

        return(
            <MultipleDatePicker>    
                <div>
                    <h1> this is calendar</h1>
                </div>
            </MultipleDatePicker>
        )
    }

```



## Roadmap

* [ ] Make it responsive
* [ ] Support for `onDateSelect` prop.
* [ ] Add test cases

## Note From Author

Hi, thanks for checking out this library. You can read more about me at https://bilalbudhani.com/about or you can follow me at https://twitter.com/BilalBudhani

