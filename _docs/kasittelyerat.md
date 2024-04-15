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

![Käsittelyerät-osioon pääsee joko Muita toimintoja -valikosta tai etusivulta Hankinnat-nappulasta](/assets/files/docs/Hankinta/kasittelyerat.png)

Käsittelyerät-toiminnolla pystyy seuraamaan erilaisi aineiston käsittelyyn liittyviä työkulkuja kuten sitomoon vientejä, ditigointia, muovitusta yms. Niteet lisätään ensin odotuslistalle, jonka jälkeen ne liitetään tarvittavaan käsittelyerään.

Jotta toimintoa voi käyttää, pitää se ensin aktivoida PreservationModule-järjestelmäasetuksesta. Myöskin odotuslistalle ja käsitelyerille pitää määrittää ei-lainata-tilan oletusarvot NOT_LOAN -auktorisoituun arvoon sekä  PreservationNotForLoanDefaultTrainIn ja PreservationNotForLoanWaitingListIn -järjestelmäasetuksiin.

## Asetukset

Asetuksissa voi määrittää kahdentyyppisiä toimintoja.

1. Yleisiin asetuksiin odotuslistan ja käsittelyerän NOT_LOAN -auktorisoidun arvon määritykset
2. Käsittelypohjat, joissa määritetään, mitä tietoja käsittelyerässä olevista niteistä näytetään

![Käsittelyerien asetukset](/assets/files/docs/Hankinta/kasittelyerat1.png)

### Yleiset asetukset

Yleisissä asetuksissa voi määrittää odotuslistan ja käsittelyerän oletusarvot NOT_LOAN -auktorisoidulle arvolle. Samat määritykset voi tehdä myös järjestelmäasetuksista PreservationNotForLoanDefaultTrainIn ja PreservationNotForLoanWaitingListIn -asetuksissa.

### Käsittelypohjat

Käsittelypohjissa määritetään, mitä tietoja niteistä näytetään käsittelyerässä. Luo uusi pohja _Lisää uusi käsittelypohja_ -napista.

![Käsittelypohjan luonti](/assets/files/docs/Hankinta/kasittelyerat1.png)

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
