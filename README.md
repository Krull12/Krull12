- 👋 Hi, I’m @Krull12
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Krull12/Krull12 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
// ==UserScript==
// @name         keydrop_giveaway_skrypt
// @namespace    https://www.cshacked.pl
// @version      1.4
// @description  KeyDrop Giveaway Bot
// @author       CSHacked.pl
// @match        https://key-drop.com/pl/giveaways/list
// @match        https://key-drop.com/pl/giveaways/list/
// @match        https://key-drop.com/pl/giveaways/keydrop/*
// @grant        none
// ==/UserScript==

(async () => {
    while (true) {
        const offset = (Math.random() + 1.2);
        await new Promise(r => setTimeout(r, 100));
        try {
            const Button_One = document.getElementsByClassName("button ml-2.5 h-11 w-28 px-3.5 text-[10px] sm:ml-4 button-light-green");
            var Button_Two = Button_One[Button_One.length - 1];
            setTimeout(() => {
                if (Button_One.lenght != 0) window.location.replace("https://key-drop.com/pl/giveaways/list/");
            }, 10000);
            if (Button_One && Button_Two) {
                Button_Two.click();
                while (true) {
                    await new Promise(r => setTimeout(r,
                        (100 * offset)));
                    try {
                        const Button_Three = document.getElementsByClassName("button mt-4 h-13 w-full whitespace-normal bg-gold text-left leading-none text-navy-900 hover:bg-gold-400 disabled:bg-navy-400 disabled:text-navy-100")[0];
                        setTimeout(() => {
                            if (Button_Three.disabled == true) window.location.replace("https://key-drop.com/pl/giveaways/list/");
                        }, 10000);
                        if (Button_Three) {
                            Button_Three.click();
                            break;
                        }
                    } catch {
                        null;
                    }
                }
            }
        } catch {
            null;
        }
    }
})();
Wejdź na stronę z Givewayami wklejając ten link w pasek adresu: https://key-drop.com/pl/giveaways/list/ i co 10 sekund będzie próbować dołączyć do konkursów
Jak wyskoczy Captcha to niestety samemu musisz ją sobie rozwiązać
1
FergusonDoświadczony
Ferguson Platynowy Hieroglif Złoty piktogram Srebrna nuta Brązowa litera Dzień Dziecka 2021
Opublikowano 24 Kwietnia
Skrypt nie działa dopóki nie dopiszę "/" na końcu linku do strony 🤔

 Cytuj
CzarnyEkspert
 Czarny Koncert życzeń Czternaście lat służby Śmieszek Efekt motyla
Opublikowano 24 Kwietnia
@Ferguson poprawione

1
 Cytuj
mati213123Nowy
mati213123 Pięć lat służby Cztery lata służby Rok służby Dwa lata służby Trzy lata służby
