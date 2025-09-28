# Mitä Sass-ominaisuuksia on käytetty ja missä

- Muuttujat (variables.scss)
  - Käytetty: 
        Värit ($color-primary, $color-secondary)
        Typografia ($font-family-base, $font-size-base, $line-height-base)
        Mitat ($spacing-unit, $border-radius, $max-width, $container-padding)

- Mixins ja include (mixins.scss)
  - mixins: button, container, respond-to (breakpoint-logiikka).
  - scss/_layout.scss käyttää @include container ja @include button, sekä @include respond-to(media) responsiivisuuteen.

- Sisäkkäiset valitsijat ja &-parent (layout.scss)
  - Käytetty rakenteelliseen tyylitykseen (esim. .site-header .main-nav .nav-link ja &.is-active).

- Osittaiset tiedostot ja import (style.css)
  - Tuodaan jokainen erikseen:
  @import 'variables', 'mixins', 'layout'

- Funktiot ja operaattorit (mixins.scss ja layout.scss)
  - Käytetty lighten(), darken() värimuutoksiin ja laskutoimituksia (esim. $spacing-unit * 2) arvojen yhdistämiseen.

- Responsiivisuus (mixins.scss ja layout.scss)
  - Käyttö: grid-rakenne (.container.grid) vaihtuu yhteen sarakkeeseen media-kyselyllä respond-to(medium).

- Komponentit (layout.scss)
  - Määritellyt komponentit: btn (button-mixinilla), hero, card, sidebar ja site-header.
    Kaikki modulaarisesti skaalattuja muuttujien avulla.

- Käännetty CSS (style.css)
  - SCSS-partialien yhdistelmä ja käännös selaimen lukemaan CSS-muotoon
  - Itse tein tällä tyylillä: 
        Suorita projektissa: npm install sass --save-dev
        Käännä: npx sass scss/style.scss css/style.css --watch
