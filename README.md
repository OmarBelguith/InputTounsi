# Input Tounsi
A jQuery plugin for entering and validating Tunisian users' data or any other data. It is made very easy to use and easier to customize.

<img src="https://raw.githubusercontent.com/Dainerx/InputTounsi/master/screenshots/screenshot-1.png?token=ASmpJW4uTy8276xSEkws2A1f28J7GRKVks5ZhmH1wA%3D%3D">

## Table of Contents

- [Demo and Examples](#demo-and-examples)
- [Features](#features)
- [Browser Compatibility](#browser-compatibility)
- [Usage](#usage)
- [Options](#options)
- [Created By](#created-by)
- [Trusted By](#trusted-by)
- [In Memory of](#in-memory-of)
- [Support and Contribution](#support-and-contribution)
## Demo and Examples
You can view [a live demo](https://jsfiddle.net/dainer/96nxdLgt/6/), or try it  yourself using the included html demo pages under the examples folder.


## Features
* Automatically validate input elements values of Tunisian user data based on default Tunisian criteria or chosen criteria.
* Automatically validate the whole form before sending request to the backend.
* Automatically display a message of error if the value entered does not match the default Tunisian criteria or chosen criteria.
* Ability to override all default options in a very simple way.

## Browser Compatibility
| Chrome | FF  | Safari | IE  | Chrome Android | Mobile Safari |
| :----: | :-: | :----: | :-: | :------------: | :-----------: | 
|    ✓   |  ✓  |    ✓   |  9  |      ✓         |       ✓       |     



## Usage

1. Include the script along with Jquery
  ```html
  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
  <script src="https://cdn.rawgit.com/Dainerx/InputTounsi/5c25d240/build/InputTounsi.min.js"></script>
  ```

2. Add the plugin script and initialise it on your input element
  ```html
  <input type="text" id="cin">
  <script>
    $("#cin").verifyInputTounsi('cin');
  </script>
  ```
3. InputTounsi supports seven kinds of input, you can only use the supported ones. 

  ```html
    <script>
    $("#name").verifyInputTounsi("name");
    $("#lastname").verifyInputTounsi("lastname");
    $("#phone").verifyInputTounsi("phone");
    $("#email").verifyInputTounsi("email");
    $("#state").verifyInputTounsi("state",$("#city"));
    $("#city").verifyInputTounsi("city");
    $("#address").verifyInputTounsi("address");
    </script>
  ```

Note: In order for state and city elements to work, you have to pass as argument your city element to verifyInputTounsi() triggered by your city element.

## Options
One of the greatest feature InputTounsi offers is overriding basically everything.

**Pattern Overriding**  
  ```html
    <script>
    $("#cin").verifyInputTounsi({
        name: "cin",
        pattern: /^(2|5|9)\d{7}$/
    });
    </script>
  ```

**Placeholder Overriding**  
  ```html
    <script>
    $("#cin").verifyInputTounsi({
        name : "cin",
        placeholder : "This is a custom placeholder, change me"
    });
    </script>
  ```

**Style Overriding**  

  ```html
    <script>
    $("#cin").verifyInputTounsi({
        name: "cin",
        styleError: [ ['border-color','yellow'],['border-style' , 'dashed'] ],
        styleSuccess: [ ['border-color','blue'],['border-style' , 'dashed'] ],
    });
    </script>
  ```
Note: You can override all css style properties following that pattern.

**Error message Overriding**  

  ```html
    <script>
    $("#cin").verifyInputTounsi({ 
        name : "cin",
        messageError: "This is a custom error message, change me!"
    });
    </script>
  ```

**Error message style Overriding**  

  ```html
    <script>
    $("#cin").verifyInputTounsi({ 
        name : "cin",
        messageErrorStyle: ['color','yellow']
    });
    </script>
  ```
Note: You can override all css style properties following that pattern.




## Created-By
- [Oussama Ben Ghorbel](http://dainer.me/)

## Trusted-By
* [Innovative Partner](http://innovativepart.com/)
* [Bugs_Bunny Team](https://www.facebook.com/BugsBunnyCTF/)


## In-Memory-Of
Farida Ben Ghorbel and Rabiaa Ben Ghorbel, lovely aunts, caring mothers and inspiring women.

## Support and Contribution

Tested InputTounsi and have comments?

* Please send your feeds back on one of my social medias accounts that can be on my [personal website](http://dainer.me/).

Interested in making InputTounsi better for everyone? 

* Come forward and contribute, everyone is welcome.

