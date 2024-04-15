---
title: 'Kohan ohje suomeksi'
permalink: /dokumentaatio/kasittelyerat/
redirect_from:
  - /theme-setup/
toc: true
---

# Käsittelyerät

Käsittelyerät-toimintoon pääset kahta reittiä.

* Etusivun Käsittelyerät-napista
* Muita toimintoja -valikosta Käsittelyerät-linkistä.

![Käsittelyerät-osioon pääsee joko Muita toimintoja -valikosta tai etusivulta Hankinnat-nappulasta](/assets/files/docs/Kasittelyerat/kasittelyerat.png)

Käsittelyerät-toiminnolla pystyy seuraamaan erilaisi aineiston käsittelyyn liittyviä työkulkuja kuten sitomoon vientejä, ditigointia, muovitusta yms. Niteet lisätään ensin odotuslistalle, jonka jälkeen ne liitetään tarvittavaan käsittelyerään.

Jotta toimintoa voi käyttää, pitää se ensin aktivoida PreservationModule-järjestelmäasetuksesta. Myöskin odotuslistalle ja käsitelyerille pitää määrittää ei-lainata-tilan oletusarvot NOT_LOAN -auktorisoituun arvoon sekä  PreservationNotForLoanDefaultTrainIn ja PreservationNotForLoanWaitingListIn -järjestelmäasetuksiin.

## Asetukset

Asetuksissa voi määrittää kahdentyyppisiä toimintoja.

1. Yleisiin asetuksiin odotuslistan ja käsittelyerän NOT_LOAN -auktorisoidun arvon määritykset
2. Käsittelypohjat, joissa määritetään, mitä tietoja käsittelyerässä olevista niteistä näytetään

![Käsittelyerien asetukset](/assets/files/docs/Kasittelyerat/kasittelyerat1.png)

### Yleiset asetukset

Yleisissä asetuksissa voi määrittää odotuslistan ja käsittelyerän oletusarvot NOT_LOAN -auktorisoidulle arvolle. Samat määritykset voi tehdä myös järjestelmäasetuksista PreservationNotForLoanDefaultTrainIn ja PreservationNotForLoanWaitingListIn -asetuksissa.

### Käsittelypohjat

Käsittelypohjissa määritetään, mitä tietoja niteistä näytetään käsittelyerässä. Luo uusi pohja _Lisää uusi käsittelypohja_ -napista.

![Käsittelypohjan luonti](/assets/files/docs/Kasittelyerat/kasittelyerat2.png)

* _Käsittelypohjan nimi_ näkyy alasvetovalikossa, kun valitaan soveltuvaa käsittelypohjaa käsittelyerälle.
* _Viestipohja kuitille_ -kohdasta valitaan, mitä viestipohjaa käytetään, kun tulostetaan käsittelyerän niteille kuitteja.
  * Jos tähän ei tee valintaa, ei niteille pysty tulostamaan kuitteja.
  * Voit käyttää joko oletusviestipohjaa PRES_TRAIN_ITEM tai luoda uuden. Muista silloin valita moduuliksi Käsittelyerät.
 
Käsittelypohjaan voi lisätä erilaisia ominaisuuksia, kuten nimeke ja tekijä. Lisää uusi ominaisuus valitsemalla _Lisää uusi määre_.

* _Nimi_: ominaisuuden/määreen nimi
* _Tyyppi_: Vaihtoehtoja on kolme: auktorisoitu arvo, tietokannan sarake tai vapaateksti
* _Valinnat_: Valintaan voi tulla eri vaihtoehtoja riippuen siitä, mitä on valittuna tyyppi-kohdassa.
  * Jos tyypissä on valittuna auktorisoitu arvo, tulee tähän lista järjestelmään tallennetuista auktorisoiduista arvoista.
  * Jos tyypissä on valittuna tietokannan sarake, tulee tähän lista käytettävissä olevista tietokannan sarakkeista, esim. biblio.title.
  * Jos tyypissä on valituna Vapaateksti, valintaa ei tule tarjolle.

Tallenna käsittelypohja _Submit_-napista.

Huom! Tyyppi ja Valinnat -riveillä toimii tietojen täydennys, eli voit alkaa kirjoittamaan kenttään haluamaasi tietoa ja valikko ehdottaa sitä vastaavia vaihtoehtoja.

Käsittelypohjia voi muokata jälkikäteen, mutta muutokset eivät päivity käsittelyeriin, jotka jo käyttävät kyseistä pohjaa. Käsittelypohja kannattaa tehdä täysin valmiiksi ennen kuin sitä käytetään käsittelyerissä.

## Odotuslista

Käsittelyerien työprosessi alkaa lisäämällä niteet odotuslistalle. Niteiden ei-lainata-tila muuttuu asetusten mukaiseksi ja on näin pois lainattavista. Niin kauan kuin niteen ei lainata -tila ei muutu, pysyy se odotuslistalla.

![Odotuslista](/assets/files/docs/Kasittelyerat/kasittelyerat3.png)

### Odotuslistalle lisääminen

Lisää niteitä odotuslistalle _Lisää odotuslistalle_ -napista.

![Odotuslista](/assets/files/docs/Kasittelyerat/kasittelyerat3.png)

Avautuu ikkuna, johon voit joko lukea tai kirjoittaa halutut viivakoodit.
