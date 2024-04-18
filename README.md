# Date-Picker

custom datepicker

daetpicker all functions.

How to use it in your application.

for see demo you first have to clone this project.

after that you can open datejquery.html file and it will showing date-picker.

add input tag with type="text" and and with any class
ex.

  <input type="text" class="datepicker" />

you can use any class in input but make sure that class should not use any where else.

then in your <script> tag
and this class should be in same class as in you input tag for date-picker

     $(".datepicker").ownDatePicker({

     <!-- here you can add your customization as you want which is mentioned below -->

    });

all functions and how to use them:

## **Date Format**

    dateFormat : string

        dateFormat: "dd-mm-yyyy"
        dateFormat: "dd/mm/yyyy"
        dateFormat: "yyyy.mm-dd"
        dateFormat: "yyyy-dd-mm"

    you can use any format or any saprator for dat format as you want

## **Default Date**

    defaultDate : number

        dafaultDate : 05
        dafaultDate : 14
        dafaultDate : 21

    set any date you want to set as the default date when date picker intiate.
    it set only date if you use only this for date and then you didnt set month and year then it will get today's month and year.

## **Default Month**

    defaultMonth : number

        defaultMonth : 02
        defaultMonth : 07
        defaultMonth : 11

    set any month you want to set as the default month when date picker intiate.
    it set only month if you use only this for month and then you didnt set date and year then it will get today's date and year.

## **Default Year**

    defaultYear : number

        defaultYear : 1867
        defaultYear : 1973
        defaultYear : 2021

    set any year you want to set as the default year when date picker intiate.
    it set only year if you use only this for year and then you didnt set date and month then it will get today's date and month.

## **Current Date**

    currentDate : string

    set current date (full date with date, month, year )

        currentDate: "20.06.2000"
        currentDate: "12.12.1836"
        currentDate: "05.02.2023"

    set any date you want which would you want to show on date-picker intiate.
    make sure that you haven't set dafaultDate, defaultMonth, defaultYear.
    if you set any of them then date will be shown as any of them.
    and also your dateformat and and current date's formate should be same.else date will be shown
    is today's date.

## **Minimum Year**

    minYear :  number

    set minimum year you want enabled and seletable.

        minYear : 1850
        minYear : 2001
        minYear : 1956

## **Maximum Year**

    maxYear :  number

    set minimum year you want enabled and seletable.

        maxYear : 1850
        maxYear : 2001
        maxYear : 1956

## **Disable Dates**

    disableDate : array

        disableDate: [ [2014, 2, 21],  [2015, 1, 15], [2017, 3, 23] ],

    add dates like this [yyyy , mm, dd] how many you want and that date will disable in date-picker and not selectable.

## **Disabel date intervals**

    disableInterval: array

        disableInterval: [
        { from: [2023, 5, 1], to: [2023, 5, 30] },
        { from: [2023, 7, 1], to: [2023, 7, 30] },
      ],

    add how many date intervals you want to disable. in this format { from: [yyyy, mm, dd], to: [yyyy, mm, dd] }
