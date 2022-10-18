<template>
  <section class="principle">
    <div class="rows">
      <div class="content-tabs">
        <!-- <div class="teaser-title">
              <h2>{{ items.title }}</h2>
        </div> -->
        <div class="full-teaser">
          <div v-for="items in items" :key="items" href="*">
            <div class="wrapper-teaser">
              <div className="teaser-block">
                <h2 class="headline">{{ items.title }}</h2>
                <div class="teaser0">
                  <img alt="vue-teaser" :src="items.img" />

                  <div class="body">
                    <div class="desc">
                      <h2>{{ items.headline }}</h2>
                      <p>{{ items.pharagraph }}</p>
                    </div>

                    <button class="btn">{{ items.button }}</button>
                  </div>
                </div>

                <div class="teaser-left">
                  <div class="teaser1">
                    <a>
                      <div class="image">
                        <img alt="vue-teaser" :src="items.img1" />
                      </div>
                      <div class="body">
                        <div class="desc">
                          <h2>{{ items.headline1 }}</h2>
                          <p>{{ items.pharagraph1 }}</p>
                        </div>

                        <button class="btn">{{ items.button }}</button>
                      </div>
                    </a>
                  </div>

                  <div class="teaser2">
                    <a>
                      <div class="image">
                        <img alt="vue-teaser" :src="items.img2" />
                      </div>
                      <div class="body">
                        <div class="desc">
                          <h2>{{ items.headline2 }}</h2>
                          <p>{{ items.pharagraph2 }}</p>
                        </div>

                        <button class="btn">{{ items.button }}</button>
                      </div>
                    </a>
                  </div>
                </div>
              </div>
              <div class="teaser-right">
                <div class="teaser3">
                  <a>
                    <div class="image">
                      <img alt="vue-teaser" :src="items.img3" />
                    </div>
                    <div class="body">
                      <div class="desc">
                        <h2>{{ items.headline3 }}</h2>
                        <div class="wrapper-stars">{{ items.star }}</div>
                      </div>

                      <div class="price">{{ items.price }}</div>
                    </div>
                  </a>
                </div>

                <div class="teaser4">
                  <a>
                    <div class="image">
                      <img alt="vue-teaser" :src="items.img4" />
                    </div>
                    <div class="body">
                      <div class="desc">
                        <h2>{{ items.headline4 }}</h2>
                        <div class="wrapper-stars">{{ items.star }}</div>
                      </div>

                      <div class="price">{{ items.price4 }}</div>
                    </div>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      items: [
        {
          //Big-Teaser
          id: "0",
          title: "Unsere Empfehlungen für Sie",
          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/graf-von-faber-castell/teaser-graf-von-faber-castell-classic.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=B2294495A6184152BA761962474BA0CB4D1A65E2",
          headline: "Graf von Faber-Castell Online-Shop",
          pharagraph:
            "Entdecken Sie unsere Luxus Kollektion mit Schreibgeräten, hochwertigsten Leder- und Schreibtischaccessoires.",
          button: "Mehr erfahren",
          star: "★★★★★",
          // middle-big-teaser
          //left
          img1: "https://www.faber-castell.de/-/media/Faber-Castell-new/special-pages/advent-2020/teaser-gravur.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=283A2DD85038F5937425179F5E8DFD12F00A9CE8",
          headline1: "Gravur direkt hier im Shop möglich",
          pharagraph1:
            "Verleihe deinem Geschenk eine persönliche Note und lasse es stilvoll gravieren!",
          // right
          img2: "https://www.faber-castell.de/-/media/Faber-Castell-new/special-pages/black-ediiton-cool/teaser-black-edition-cool-neu.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=D337C181E6C416333D97164663A71FD3E03A2471",
          headline2: "Cooles Upgrade fürs Homeoffice: ",
          pharagraph2:
            "Dieser Look trifft voll ins Schwarze: Der dunkle Schaft lässt den bunten Farben die Bühne und .",
          //Right Side of Teasers
          // top
          img3: "https://www.faber-castell.de/-/media/Products/Product-Repository/Watercolour-Marker/24-25-04-Fibre-tip-pen/160320-Watercolour-marker-ADrer-20ct-wallet/Images/160320_10_PM1.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=3F09D867137ADEF6674BADB06ACAD356EF3F0D52",
          headline3: "Albrecht Dürer Watercolour Marker, 20er Etui",
          price: "80,00 €",
          // bottom
          img4: "https://www.faber-castell.de/-/media/Products/Product-Repository/Mixed-displays/24-33-12-Sets/201847-Starter-parcel-for-beginners/Images/201847_10_PM1.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=0F23F631012423499848CCA064F1A4E2D1288048",
          headline4: "Schulstarter Set",
          price4: "49,00 €",
        },
        // Second Teaser
        {
          id: "1",
          title:
            "Erfahren Sie mehr über unsere ökologischen und sozialen Projekte",
          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/sustainability/2020/teaser-eco.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=0544BFDD06BF22926EBE0857B9C4C961E529032B",
          headline: "Ökologisch",
          pharagraph:
            "Unsere unternehmenseigenen Wälder in Brasilien leisten einen großen Beitrag.",
          button: "Mehr erfahren",
          star: "★★★★★",
          // middle-big-teaser
          //left
          img1: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/sustainability/factsheets/teaser-fact-sheets.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=611EB581660A25972106B73C5671E648DE344624",
          headline1: "Nachhaltigkeit – Fact Sheets",
          pharagraph1:
            "Mehr Informationen finden Sie zusammengefasst in unseren Nachhaltigkeit - Fact Sheets. ",
          // right
          img2: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/sustainability/2020/teaser-social.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=9D01C79B3026824CCA21CF954255484FBA391660",
          headline2: "Soziales",
          pharagraph2:
            "Für uns ist soziales Engagement schon seit vielen Generationen Teil der unternehmerischen Verantwortung.",
          //Right Side of Teasers
          // top
          img3: "https://www.faber-castell.de/-/media/Products/Product-Repository/Colour-GRIP/24-25-03-Colored-pencil/112442-Col,-d-,-pencil-Colour-GRIP-cardboard-36x/Images/112442_10_PM1.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=7AE2FDDB8B982D24BEB3EFFB4B8A5C99B4B2ADD1",
          headline3: "Colour Grip Buntstift, 36er Kartonetui",
          price: "30,00 €",
          // bottom
          img4: "https://www.faber-castell.de/-/media/Products/Product-Repository/Polychromos-artists-colour-pencils/24-25-03-Colored-pencil/110006-Polychromos-colour-pencil-wooden-case-of-48/Images/110006_10_PM1.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=5838A740F3701FC2D86ABAFB013652CDFC84D574",
          headline4: "Polychromos Farbstift, 48er Holzkoffer",
          price4: "150,00 €",
        },

        // Third Teaser
        {
          id: "2",
          title: "Stöbern Sie in unserem neuen Magazin",
          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/magazin/teaser-aerial_view.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=A556BAE7AB5088C8BA3FE58B950BEED527B2043E",
          headline: "Vom Baum zum Bleistift",
          pharagraph:
            "Unsere holzgefassten Stifte stammen überwiegend aus firmeneigenen Wäldern in Brasilien.",
          button: "Mehr erfahren",
          star: "★★★★★",
          // bottom-big-teaser
          //left
          img1: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/magazin/small-pen-big-impact/teaser-wooden_pencil.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=25E3415A44E79D4FAB955319DD27779E05102235",
          headline1: "Kleiner Stift, ganz groß",
          pharagraph1:
            "Fünf Facts über einen Alleskönner – in der Mode, in Hollywood, im Rekordhalten.",
          // right
          img2: "https://www.faber-castell.de/-/media/Faber-Castell-new/Corporate/magazin/interview-with-ceo/teaser-ceo.ashx?mh=303&la=de-DE&h=303&w=536&mw=540&hash=7F577D33BB70A2EDA768E4FBEEFB3E2E0EB09CA2",
          headline2: "Interview mit CEO Stefan Leitz",
          pharagraph2:
            "Seit März 2020 ist Stefan Leitz Vorstandsvorsitzender von Faber-Castell.",
          //Right Side of Teasers
          // top
          img3: "https://www.faber-castell.de/-/media/Products/Product-Repository/Polychromos-artists-colour-pencils/24-25-03-Colored-pencil/110013-Pencil-Polychromos-CASE120/Images/110013_10_PM1.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=8673ED47054A5547C6E79C1FF09B5219451E6D89",
          headline3: "Polychromos Farbstift, 120er Holzkoffer",
          price: "395,00 €",
          // bottom
          img4: "https://www.faber-castell.de/-/media/Products/Product-Repository/PITT-Monochrome-Graphite/24-24-01-Pencil/117806-Watsol-pencil-GRAPHITE-AQUARELLE-6B/Images/117806_0_PM99.ashx?bc=ffffff&w=273&h=290&as=0&la=de-DE&hash=EE0469E9493FA6E294BDB54D221A20F974AC7361",
          headline4: "Polychromos Farbstift, 120er Holzkoffer",
          price4: "35,00 €",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.wrapper-teaser {
  display: flex;
  max-width: 1028px;
  margin: 0 auto;
  padding-bottom: 70px;
  padding-top: 70px;

  .headline {
    color: #05301a;
    font-family: "Times New Roman", Times, serif;
    font-size: 24px;
    font-style: italic;
    letter-spacing: 0.01em;
    line-height: 28px;
    display: inline-block;
    float: none;
    margin-left: 12px;
    width: auto;
    font-weight: normal;
  }

  .wrapper-stars {
    color: orange;
    font-size: 20px;
  }

  .price {
    color: #707170;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px;
  }
}

.teaser-block {
  width: 85%;

  .teaser0 {
    display: flex;
    margin-right: 10px;
    margin-bottom: 10px;
  }
}
.teaser0:hover {
  box-shadow: 0 0 13px 0 rgb(18 24 28 / 30%);
  cursor: pointer;
}

.teaser-left {
  display: flex;

  .teaser1 {
    margin: 10px;
    margin: 10px;
    transition: 0.2s cubic-bezier(0.55, 0.06, 0.68, 0.19);
    background-color: #ffffff;
    margin-bottom: 12px;
    position: relative;
    text-align: left;
    text-decoration: none;
    vertical-align: top;
    width: 50%;

    img {
      width: 379px;
      height: 214px;
    }
    .image {
      box-sizing: border-box;
      background: #ffffff;
      overflow: hidden;
      padding: 0;
      position: relative;
      text-align: center;
      z-index: 70;
    }
  }

  .teaser1:hover {
    box-shadow: 0 0 13px 0 rgb(18 24 28 / 30%);
    cursor: pointer;
  }
  .teaser2 {
    margin: 10px;
    margin: 10px;
    transition: 0.2s cubic-bezier(0.55, 0.06, 0.68, 0.19);
    background-color: #ffffff;
    margin-bottom: 12px;
    position: relative;
    text-align: left;
    text-decoration: none;
    vertical-align: top;
    width: 50%;

    img {
      width: 379px;
      height: 214px;
    }
    margin: 10px;
    .image {
      background: #ffffff;
      box-sizing: border-box;
      overflow: hidden;
      padding: 0;
      text-align: center;
      z-index: 70;
    }
  }
  .teaser2:hover {
    box-shadow: 0 0 13px 0 rgb(18 24 28 / 30%);
    cursor: pointer;
  }
}

.teaser-right {
  margin-top: 55px;

  .teaser3 {
    transition: 0.2s cubic-bezier(0.55, 0.06, 0.68, 0.19);
    background-color: #ffffff;
    margin-bottom: 12px;
    position: relative;
    text-align: left;
    text-decoration: none;
    vertical-align: top;

    .image {
      height: 300px;
      padding: 10px 0 0 0;
      box-sizing: border-box;
      background: #ffffff;
      overflow: hidden;
      padding: 0;
      position: relative;
      text-align: center;
      z-index: 70;
    }

    img {
      width: 273px;
      height: 290px;
    }
  }
  .teaser3:hover {
    box-shadow: 0 0 13px 0 rgb(18 24 28 / 30%);
    cursor: pointer;
  }

  .teaser4 {
    transition: 0.2s cubic-bezier(0.55, 0.06, 0.68, 0.19);
    background-color: #ffffff;
    margin-bottom: 12px;
    position: relative;
    text-align: left;
    text-decoration: none;
    vertical-align: top;

    .image {
      height: 300px;
      padding: 10px 0 0 0;
      box-sizing: border-box;
      background: #ffffff;
      overflow: hidden;
      padding: 0;
      position: relative;
      text-align: center;
      z-index: 70;
    }

    img {
      width: 273px;
      height: 290px;
    }
  }
  .teaser4:hover {
    box-shadow: 0 0 13px 0 rgb(18 24 28 / 30%);
    cursor: pointer;
  }
}
.body {
  /*    
        padding: 15px 12px 12px 22px;
        box-sizing: border-box;
      
      
        background-color: white; */

  background-color: #ffffff;
  margin-bottom: 8px;
  margin-top: 0;
  padding: 0 20px 0 20px;
  z-index: 80;

  h2 {
    color: #05301a;
    font-family: "Times New Roman", Times, serif;
    font-size: 20px;
    letter-spacing: 0.01em;
    line-height: 24px;
    overflow: hidden;
    position: relative;
    max-height: 48px;
    margin-bottom: 11px;
    font-weight: normal;
  }
}
</style>
