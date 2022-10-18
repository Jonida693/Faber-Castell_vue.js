<template>
  <section class="navigation-footer">
    <div class="footer-section row">
      <div class="col-md-3" v-for="menus in menus" :key="menus" href="*">
        <div class="footer-menus">
          <div class="menus-first-col">
            <h3>{{ menus.menu }}</h3>
            <ul>
              <li>{{ menus.sub1 }}</li>
              <li>{{ menus.sub2 }}</li>

              <li>{{ menus.sub3 }}</li>

              <li>{{ menus.sub4 }}</li>

              <li>{{ menus.sub5 }}</li>

              <li>{{ menus.sub6 }}</li>

              <li>{{ menus.sub7 }}</li>

              <li>{{ menus.sub8 }}</li>

              <li>{{ menus.sub9 }}</li>

              <li>{{ menus.sub10 }}</li>

              <li>{{ menus.sub11 }}</li>

              <li>{{ menus.sub12 }}</li>

              <li>{{ menus.sub13 }}</li>

              <li>{{ menus.sub14 }}</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="total-links">
      <ul>
        <li>Allgemeine Geschäftsbedingungen</li>
        <li>Datenschutzerklärung der Faber-Castell Unternehmensgruppe</li>
        <li>Länderauswahl</li>
      </ul>
    </div>

    <div class="copyright">
      <ul>
        <li>Copyright 2022 Faber-Castell. All Rights reserved.</li>
        <li>Impressum</li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      menus: [
        {
          //First colon
          id: "0",

          menu: "Online einkaufen",
          sub1: "Bleistifte",
          sub2: "Buntstifte und Künstlerfarbstifte",
          sub3: "Füllfederhalter",
          sub4: "Tintenroller",
          sub5: "Fineliner und Filzstifte",
          sub6: "Wasserfarben und Zubehör",
          sub7: "Kugelschreiber",
          sub8: "Kreiden",
          sub9: "Zirkel",
          sub10: "Technisches Zeichnen",
          sub11: "Radiergummis",
          sub12: "Spitzer",
          sub13: "Zubehör",
          sub14: "Minen und Tinten",
        },

        //second colum

        {
          id: "1",
          menu: "Inspiration",
          sub1: "Künstler",
          sub2: "Kinder",
          sub3: "Für Lehrer und pädagogische",
          sub4: "Fachkräfte",
          sub5: "Videos für Künstler",
          sub6: "Videos für Kinder",
          sub7: "Videos: Schule - Studium - Beruf",
        },
        //third colum

        {
          id: "2",

          menu: "Unternehmen",
          sub1: "Nachhaltigkeit",
          sub2: "Faber-Castell Erleben",
          sub3: "Historie",
          sub4: "Unternehmensgrundsätze",
          sub5: "Zahlen & Fakten",
        },
        //fourth colum

        {
          id: "3",

          menu: "Service",
          sub1: "Servicehotline: +49 911 9965 0",
          sub2: "Shophotline: +49 911 9965 8888",
          sub3: "Ersatzteile",
          sub4: "Presse",
          sub5: "Mediadatenbanken",
          sub6: "Adressen weltweit",
          sub7: "Lieferung & Versand",
          sub8: "Bezahlung und Sicherheite",
          sub9: "Rücksendung und Rückerstattung ",
          sub10: "Garantie",
          sub11: "Lieferantenbewerbung",
          sub12: "Supplier Application",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.navigation-footer {
  max-width: 1280px;
  margin: 0 auto;
  .footer-section {


    h3 {
      color: #05301a;
      font-family: "Times New Roman", Times, serif;
      font-size: 20px;
      font-style: italic;
      letter-spacing: 0.035em;
      line-height: 32px;
      font-weight: normal;
      padding: 0;
    }
    ul {
      list-style: none;
      margin: 0;
      padding: 0;
      li {
        color: #707170;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 12px;
        letter-spacing: 0.035em;
        line-height: 27px;
        margin-bottom: 15px;
        text-decoration: none;
      }
    }
  }
}

.total-links {
  border-top: 1px solid #e2e3e3;

  ul {
    display: flex;
    justify-content: space-between;
    li {
      text-decoration: none;
      list-style: none;
      color: #05301a;
      cursor: pointer;
      float: left;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 14px;
      letter-spacing: 0.035em;
      line-height: 26px;
      padding-top: 22px;
      padding-right: 22px;
      margin-right: 22px;
      position: relative;
      text-decoration: none;
    }
  }
}

.copyright {
  border-top: 1px solid #e2e3e3;

  ul {
    display: flex;
    justify-content: space-between;
    li:first-child {
      opacity: 0.5;
      filter: alpha(opacity=50);
      color: #707170;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 12px;
      letter-spacing: 0.035em;
      line-height: 19px;
      display: inline-block;
      margin: 28px 34px 28px 6px;
      vertical-align: middle;
    }

    li {
      opacity: 0.5;
      filter: alpha(opacity=50);
      color: #05301a;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 12px;
      letter-spacing: 0.035em;
      line-height: 19px;
      display: inline-block;
      margin: 28px 34px 28px 6px;
      vertical-align: middle;
    }
  }
}
</style>
