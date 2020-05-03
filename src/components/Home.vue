<template>
    <div id="home">
        <h1 class="title display-bold">Meal planning<br>made easy!</h1>
        <p class="subtitle display-normal">Life is hectic, planning your meals don't have to be.</p>
        <ul class="checklist">
        <li>Build weekly menus</li>
        <li>Create and import recipes</li>
        <li>Save time and money, eliminate food waste</li>
        <li>Thousands of keto and low-carb-friendly ingredients</li>
        </ul>
        <p class="text">Take control of your time by using Avokado, a clean and simple meal planning platform made for people who trust in real food. Get warned if an ingredient isn't keto or low-carb-friendly, we'll even show you a better alternative!</p>
        <div id="signup">
            <form>
                <div class="checkme">
                    <p class="checkbox-label">Let me know when avokado.health is available: </p>
                    <input type="checkbox" id="checkbox" v-model="signMeUp" >
                    <label for="checkbox"></label>
                </div>
            </form>
            <Mailchimp v-if="signMeUp == true" />
        </div>
    </div>
</template>

<script>
import Mailchimp from './Mailchimp';
export default {
  name: 'Home',
  components: {
      Mailchimp
  },
  data() {
      return {
        signMeUp: ''
      }
  }
}
</script>

<style lang="scss">
@import '../sass/_vars';

    #home {
        width: 70%;
    }

    .checklist {
        padding-bottom: 1rem;

        li {
            margin-bottom: 1rem;
        }

        li:before {
            content: "\2714";
            margin-right: 1rem;
            color: $gray;
        }
    }

    .text {
        margin-top: 3rem;
    }
    
    #checkbox {
       
    }    

    input[type=checkbox] { 
        display:none; 
    } /* to hide the checkbox itself */

    input[type=checkbox] + label:before {
        display: inline-block;
        margin-left: 1rem;
    }

    /* unchecked icon */
    input[type=checkbox] + label:before { 
        content: ""; 
        background-color: black;
        display: inline-block;
        position: relative;
        width: 30px;
        height: 30px;
        border-radius: 50%;
        font-size: 2rem;
    } 

    input[type=checkbox]:checked + label:before { 
        content: "\2714"; 
        color: #91E2A3; 
        font-size: 2rem;
        padding-left: 0.5rem;
        line-height: 1.25rem;

    } /* checked icon */

    #signup {
        margin-top: 4rem;
        .checkbox-label {
            font-family: 'urw_din_bold', sans-serif !important;
            display: inline-block;
            line-height: 1.5rem;
            font-size: 2rem;
        }

        form .checkme{
            position: relative;
            display: flex;
            align-content: center;
        }
    }

    .indicates-required {
        font-size: 0.75rem;
        font-family: 'urw_din_bold', sans-serif !important;
        color: #FF004E;
    }
</style>