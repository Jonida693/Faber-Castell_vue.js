<template>
  <section class="white-section">
    <div class="primary-colon row">
      <div class="newsletter col-md-4">
        <div class="footer-newsletter">
          <h3>Newsletter</h3>
          <p>
            Erhalten Sie alle Neuigkeiten direkt per E-Mail und sichern Sie sich
            Ihren

            <strong>10% Willkommensgutschein</strong>
          </p>
          <h4>(ab 50 Euro Warenwert)</h4>
        </div>

        <div class="input-form">
          <label class="label">Confirm email address</label>
          <input E-mail address />

          <button>Anmelden</button>
        </div>

        <p class="description">
          Ja, ich möchte den Faber-Castell Newsletter erhalten. Weitere
          Informationen können Sie der Datenschutzerklärung entnehmen. Ihre
          Einwilligung in den Versand ist jederzeit widerruflich (durch Klick
          auf den in jeder Newsletter E-Mail bereitgestellten Abmeldelink.
        </p>
      </div>

      <div class="social-media col-md-4">
        <h3>Folgen Sie uns auf</h3>
        <p>Tipps, Tutorials und Inspiration auf Social Media</p>

        <div class="social-icons">
          <a href="fs">
            <img
              src="https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Footer-facebook-grey.ashx"
            />
          </a>

          <a href="fs">
            <img
              src="https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Footer-Instagram-grey.ashx"
            />
          </a>

          <a href="fs">
            <img
              src="https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Footer-Youtube-grey.ashx"
            />
          </a>

          <a href="fs">
            <img
              src="https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Footer-Pinterest-grey.ashx"
            />
          </a>
        </div>
      </div>

      <div class="third-col col-md-4">
        <h3>Händlersuche</h3>
        <p>Finden Sie einen Händler in Ihrer Nähe</p>
        <div>
          <button>Geschäft suchen</button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  social: [{}],
};
</script>

<style lang="scss">
.white-section {
  background-color: #ffffff;

  .primary-colon {
    display: flex;
    margin: 0 auto;
    max-width: 1280px;
      padding-top: 110px;

    button {
      border-radius: 3px;
      background: rgb(198, 188, 151);
      border: none;
      color: #ffffff;
      cursor: pointer;
      display: inline-block;
      font-family: Arial, Helvetica, sans-serif;
      font-size: 14px;
      letter-spacing: 0.035em;
      line-height: 21px;
      margin-top: 26px;
      padding: 10px 14px 10px;
      opacity: 1;
      margin-left: 20px;
    }
    .newsletter {
      .footer-newsletter {
        h3 {
          color: #05301a;
          font-family: "Times New Roman", Times, serif;
          font-size: 24px;
          font-style: italic;
          letter-spacing: 0.01em;
          line-height: 28px;
          margin-bottom: 11px;
          font-weight: normal;
        }

        p {
          color: #707170;
          font-family: Arial, Helvetica, sans-serif;
          font-size: 14px;
          letter-spacing: 0.035em;
          line-height: 21px;
          margin-bottom: 15px;
        }

        h4 {
          opacity: 0.5;
          filter: alpha(opacity=50);
          color: #707170;
          font-family: Arial, Helvetica, sans-serif;
          font-size: 12px;
          letter-spacing: 0.035em;
          line-height: 19px;
          clear: both;
          margin-top: 5px;
        }
      }
      .input-form {
        position: relative;

        input {
          padding: 10px 0;
        }
        label.label {
          position: absolute;
          bottom: 10px;
          font-size: 13px;
          margin-left: 10px;
        }
      }

      .description {
        opacity: 0.5;
        filter: alpha(opacity=50);
        color: #707170;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 12px;
        letter-spacing: 0.035em;
        line-height: 19px;
        clear: both;
        float: left;
        margin-top: 5px;
      }
    }
    .social-media {
      p {
        color: #707170;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 14px;
        letter-spacing: 0.035em;
        line-height: 21px;
        margin-bottom: 15px;
      }
      h3 {
        color: #05301a;
        font-family: "Times New Roman", Times, serif;
        font-size: 24px;
        font-style: italic;
        letter-spacing: 0.01em;
        line-height: 28px;
        margin-bottom: 11px;
        font-weight: normal;
      }

      .social-icons {
        display: flex;
        a {
          margin-right: -27px;
        }
        img {
          max-width: 30px;
          margin: 0 32px;
        }
      }
    }

    .third-col {
      h3 {
        color: #05301a;
        font-family: "Times New Roman", Times, serif;
        font-size: 24px;
        font-style: italic;
        letter-spacing: 0.01em;
        line-height: 28px;
        margin-bottom: 11px;
        font-weight: normal;
      }
    }
  }
}
</style>
