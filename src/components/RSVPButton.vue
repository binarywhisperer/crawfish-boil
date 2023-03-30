<template>
  <section class="rsvp">
    <section class="rsvp-tuple">
      <div class="rsvp-tuple--div">
        <figure>
          <img alt="RSVP and 2 Crawfish" src="../assets/rsvp.png"/>
        </figure>
      </div>
      <div class="rsvp-tuple--button--wrapper rsvp-tuple--div">
        <div>
          <p>RSVP when you pay through PayPal. Add multiples in PayPal interface. Don't forget to come back for your drinks</p>
          <div class="rsvp-tuple--button">
            <section>
              <h2>Food Selection</h2>
              <form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post" >
                <input type="hidden" name="cmd" value="_s-xclick">
                <table>
                  <tr><td><select class="select is-large" name="os0">
                  <option value="Crawfish and Sides">Crawfish and Sides $20.00 USD</option>
                  <option value="Sides Only">Sides Only $10.00 USD</option>
                </select> </td></tr>
                </table>
                <input type="hidden" name="encrypted" value="-----BEGIN PKCS7-----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-----END PKCS7-----">
                <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
                <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
              </form>
              <hr/>
            </section>
            <section>
              <h2>Drink Selection</h2>
              <span>(single charge, not per drink, access to cooler)</span>
              <form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post" >
                <input type="hidden" name="cmd" value="_s-xclick">
                <table>
                  <tr><td><select name="os0" class="select is-large">
                  <option value="Drinks - Alcoholic">Drinks - Alcoholic $5.00 USD</option>
                  <option value="Drinks - Non-Alcoholic">Drinks - Non-Alcoholic $2.00 USD</option>
                </select> </td></tr>
                </table>
                <input type="hidden" name="encrypted" value="-----BEGIN PKCS7-----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-----END PKCS7-----">
                <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
                <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
              </form>
              <hr/>
            </section>
            <section>
              <h2>View Cart</h2>
              <form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post" >
                <input type="hidden" name="cmd" value="_s-xclick">
                <input type="hidden" name="encrypted" value="-----BEGIN PKCS7-----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-----END PKCS7-----">
                <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_viewcart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
                <img alt="" border="0" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
              </form>
            </section>
          </div>
        </div>
      </div>
    </section>
  </section>
</template>

<script>
export default {
  name: 'RSVPButton',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.rsvp{
  background: white;
}
.rsvp-tuple{
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  &--div{
    width: 40%;
    min-width: 400px;
  }

  &--button{
    td{
      border: none!important;
    }
    h2{
      margin-bottom: 0;
    }
    section {
      margin-bottom: 1rem;
    }

    &--wrapper{
      width: 59%;
      display: flex;
      justify-content: center;
      padding: 2rem .5rem;
      div p{
        font-weight: 700;
        font-size: 1.25rem;
      }
    }
    button{
      background: #550000;
      color: white;
    }
  }
}
</style>
