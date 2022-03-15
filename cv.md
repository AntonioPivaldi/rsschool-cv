## 1: Name and surname
*Vladislav Yakushev*
## 2: Contacts:
    - Phone number: +375 29 891-30-03;
    - E-mail: 9212565@gmail.com;
    - VK: https://vk.com/redrop;
    - Instagram: https://instagram.com/vselenskiy_otets;
    - Discord nickname: Pivaldi#2497.

## 3: About me
Well, I'm 23 y. o., finished school in 2015 and entered in medical university in the same year. I enjoy cooking (average cooking enjoyer, ye). I really like to play a *guitar*, watch some *movies* and play *videogames*. My *life goal* is to make a world around me more *advanced* and *improved*, at least a little bit, even though it sounds so maximalistic. I graduated from medical uni and at the moment I'm an *internist*, working at hospital during my internship. Also I've completed *JS/FE Pre-School* 2022. Now will try to fight with Stage 1 of *JS/FE 2022Q1*.

## 4: My skills
    - HTML, CSS;
    - SASS, WebPack;
    - Basics in JavaScript;
    - Basics in Git, GitHub;
    - VS Code;
    - Basics in Photoshop;
    - Fundamental skills in medicine.

## 5: Code sample
// Setting variables

const urlEng = 'https://type.fit/api/quotes';

const urlRus = require('./assets/packages/quotes-rus.json');

let buttonSound = document.querySelector('.quoter-button-sound');

let quoterText = document.querySelector('.quoter-text');

let quoterAuthor = document.querySelector('.quoter-author');

let quoterImage = document.querySelector('.quoter-image > img');

let engQuote;

let rusQuote;

let engAuthor;

let rusAuthor;

buttonSound.src = document.querySelector('.quoter-button-sound').src;

buttonSound.load();


window.newQuote = async () => {

    // VFX and SFX

    buttonSound.play();

    quoterImage.src = document.querySelector('.quoter-image > img').src;

    getData();

}

// Geting quote text

async function getData() {

    const resEng = await fetch(urlEng);

    let dataEng = await resEng.json();

    function getText() {

        let numberEng = Math.floor(Math.random() * dataEng.length);

        let numberRus = Math.floor(Math.random() * urlRus.length);

        engQuote = dataEng[numberEng].text;

        rusQuote = urlRus[numberRus].text;

        engAuthor = dataEng[numberEng].author;

        rusAuthor = urlRus[numberRus].author;

        if (currentLang === 'eng') {

            quoterText.textContent = engQuote;

            quoterAuthor.textContent = engAuthor;

        }

        else {

            quoterText.textContent = rusQuote;

            quoterAuthor.textContent = rusAuthor;

        }

    }

    getText();

}

getData();

## 6: Experience
- https://antoniopivaldi-rs-portfolio.netlify.app
- https://antoniopivaldi-rs-audioplayer.netlify.app
- https://antoniopivaldi-rs-quotes.netlify.app
- https://antoniopivaldi-rs-tictactoe.netlify.app (unfinished collab with Zidiks)
- Also at the moment I have an experience in *medicine*, primarily in *surgery*, can provide a hemorrhoidectomy.
## 7: Education:
    - Mid-school from 2003 to 2015;
    - Vitebsk State Medical University from 2015 to 2021;
    - Surgical internship from august 2021 and still lasts;
    - JS/FE Pre-School 2021;
    - JS/FE 2022Q1 from 13.03.2022 and still lasts.

## 8: English level
There are no any official certificates to prove my English level, but I'm always *trying to do my best*.