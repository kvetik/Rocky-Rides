// SCSS

html { box-sizing: border-box; }
*, ::before, ::after { box-sizing: inherit; }

* {
    margin: 0;
    padding: 0;
}

//Variables//
$c-text: #004167;
$c-button: #fed766;
$background: #f4f4f9;

body {
    font-family: Nunito sans, sans-serif;
    font-size: 16px;
    color: $c-text;
}

h1, h2, h3 {
    font-family: Paytone One, sans-serif;
}

h1 {
    font-size: 36px;
    //text-decoration: underline ;//
    //text-underline-position: under;//
}

h2 {
    font-size: 22px;
    font-weight: 200;
    padding-bottom: 10px;
}

h3 {
    font-size: 18px;
    font-weight: 100;
}

ul {
    list-style: none;
  }

// Input - Submit button
input[type="submit"] {
    color: $c-text;
    font-size: 16px;
    font-weight: bold;
    padding: 10px;
    margin-top: 10px;
    background-color: $c-button;
    border-radius: 20px;
    border: none;
    text-align: center;
    cursor: pointer;
  }

  input[type="submit"]:hover {
    color: $c-button;
    background-color: $c-text;
  }


// Button
.button {
    color: $c-text;
    font-size: 16px;
    font-weight: bold;
    padding: 10px;
    margin-top: 10px;
    background-color: $c-button;
    border-radius: 20px;
    border: none;
    text-align: center;
    cursor: pointer;
}

.button:hover {
    color: $c-button;
    background-color: $c-text;
}


// Header
.header__top {
    margin: 0;
    padding: 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header__left {
    width: 60%;  
    display: flex;
    align-items: center;

    .header__title {
        width: 700px;
        height: auto;
      }
      
      .header__logo {
        width: 200px;
        height: auto;
      }
}

.header__right {
    width: 30%;
    text-align: center;
    display: flex;
    flex-direction: column;
    
    .quote {
        padding-bottom: 20px;
        font-size: 20px;
        font-style: italic;
        transform: rotate(-15deg);
    }
}

// Menu
.menu__all {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
    background-color: $c-text;
    border-radius: 20px;
}

.menu__list {
	list-style: none;
	margin: 0 auto;
	padding: 0;
	display: flex;
    justify-content: space-between;
    gap: 50px;
}

.menu__item {
	margin: 0;
	padding: 0 40px;
    flex-grow: 1;
}

.menu__link {
	display: block;
	padding: 10px;
	font-size: 20px;
	font-weight: bold;
	text-decoration: none;
	color: white;
}

.menu__link:hover {
	background-color: $c-button;
    color: $c-text;
    border-radius: 10px;
}

.menu__banner {
    width: 100%;
}

// Content - Welcome page
.content__welcome {
    background-color: $background;
    display: flex;
    justify-content: space-between;
    padding: 10px;
    gap: 10px;

    .introduction, .review {
        flex: 1 1 50%;
        text-align: center;
        background-color: white;
        border-radius: 20px;
        padding: 30px;
        margin: 10px;
    }

    .introduction {
        line-height: 2;
    }
}

.review {
    display: flex;
    flex-direction: column;
    gap: 20px;

    .review__row {
        display: flex;
        gap: 20px;
        margin-bottom: 40px;
    
        .review__row--vert {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .review__row--vert img {
            max-width: 100%;
            height: auto;
        }
        
        .review__row--vert:nth-child(2) {
            flex-direction: column-reverse;
        }
    }

    .review__horiz {
        display: flex;
        flex-direction: row;
    }

    .review__description {
        padding: 20px;
    }
}

// Tours
.tours__title {
        background-color: white;
        border-radius: 20px;
        text-align: center;
        margin-bottom: 20px;
        padding: 10px;
}

.tours {
    background-color: $background;
    display: flex;
    overflow-x: auto;

    .tour {
        flex: 1 1 25%;
        text-align: center;
        margin: 10px;
        padding: 30px;
        background-color: white;
        border-radius: 20px;

        .tour__description {
            line-height: 2;
        }
    }
}

// Content - About and Contact page
.content__about {
    display: flex;
    background-color: $background;
    justify-content: space-between;
    padding: 10px;
    gap: 10px;

    .about, .contact {
        flex: 1 1 50%;
        text-align: center;
        background-color: white;
        border-radius: 20px;
        padding: 30px;
        margin: 10px;
        line-height: 2;
    }
    
    .contact__detail img {
        padding: 20px;
    }
    .contact__message {
        background-color: white;
        padding: 20px;
        margin: 0 auto;   
    }

    textarea {
        width: 90%;
        height: 200px;
        margin: 30px;
        border: 2px solid $c-button;
        border-radius: 20px;
      }
}

// Booking page
.booking__title {
    background-color: white;
    border-radius: 20px;
    text-align: center;
    margin-bottom: 20px;
    padding: 10px;
}

.content__booking {
    display: flex;
    background-color: $background;
    justify-content: space-between;
    padding: 10px;
    gap: 10px;

    .form, .customer {
        flex: 1 1 50%;
        text-align: center;
        background-color: white;
        border-radius: 20px;
        padding: 30px;
        margin: 10px;
        line-height: 2;
    }
}

.form__tour {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 20px;
}

.customer__info--form {
    text-align: left;
    padding-left: 60px;
}

label {
	display: block;
	
}

input[type="text"],
input[type="email"],
input[type="tel"],
input[type="number"] {
	width: 400px;
	padding: 20px;
	border: 2px solid $c-button;
	border-radius: 20px;
    margin-bottom: 10px;
}

input::placeholder {
	color: $c-text;
	font-style: italic;
}

// Calendar
h3 {
    text-align: center;
    color: $c-text;
    display: flex;
    justify-content: space-around;
}
span {
    cursor: pointer;
}
.container {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}
.calendar {
    color: $c-text;
    background-color: white;
    max-width: fit-content;
	border: 2px solid $c-text;
	border-radius: 20px;
}

.calendar div {
    text-align: center;
}

table {
    text-align: center;
	padding: 0 20px 20px 20px;
}
th {
	padding: 0 10px 10px 10px;
}

td {            
    cursor: pointer;
    font-family: Nunito sans, sans-serif;
    font-size: 16px;
}
.current {
    background-color: $c-button;
    color: $c-text;
    border-radius: 50%;
}

// Footer
.footer {
    color: $c-text;
    font-size: 16px;
    font-weight: bold;
    background-color: $c-button;
    text-align: center;
}