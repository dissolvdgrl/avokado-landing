<template>
    <!-- Begin Mailchimp Signup Form -->
    <div id="mc_embed_signup">
        <form action="https://chilldsgn.us8.list-manage.com/subscribe/post?u=a7cc466d17bc8391e7175f91f&amp;id=e037cfa691" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
            <div id="mc_embed_signup_scroll">
            <h2></h2>
            <div class="indicates-required"><span class="asterisk">*</span> indicates required</div>
            <div class="mc-field-group">
                <input type="text" value="" name="FNAME" class="form-input" id="mce-FNAME">
                <label for="mce-FNAME">First Name </label>
            </div>
            <div class="mc-field-group">
                <input type="text" value="" name="LNAME" class="form-input" id="mce-LNAME">
                <label for="mce-LNAME">Last Name </label>
            </div>
            <div class="mc-field-group">
                <input type="email" value="" name="EMAIL" class="required email form-input" id="mce-EMAIL">
                <label for="mce-EMAIL">Email Address  <span class="asterisk">*</span>
            </label>
            </div>
            <div id="mce-responses" class="clear">
                <div class="response" id="mce-error-response" style="display:none"></div>
                <div class="response" id="mce-success-response" style="display:none"></div>
            </div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
            <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_a7cc466d17bc8391e7175f91f_e037cfa691" tabindex="-1" value=""></div>
            <div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
            </div>
        </form>
        <p class="form-disclaimer">Unsubscribe whenever you want</p>
    </div>

    <!--End mc_embed_signup-->
</template>

<script>
 export default{
     
 }
</script>

<style>
    .mc-field-group {
        padding: 1rem 0;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
    }

    .mc-field-group label {
        font-size: 1rem;
        font-family: 'calgary_serial', serif;
    }

    .form-input {
        background-color: transparent;
        border: none;
        border-bottom: 2px solid black;
        width: 50%;
        margin-top: 1rem;
        font-size: 1.5rem;
    }

    p.form-disclaimer {
        font-family: 'calgary_serial', serif;
        font-size: 0.75rem;
    }

    .asterisk {
        color: #FF004E;
    }

    .button {
        border-radius: 0px;
        border: 0;
        background-color: #3E3E3E;
        color: #91E2A3;
        font-family: 'calgary_serial', serif;
        font-weight: bold;
    }

    .button:hover {
        opacity: 0.8;
        color: #91E2A3;
    }
</style>