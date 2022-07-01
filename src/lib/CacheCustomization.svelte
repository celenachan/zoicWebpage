<script>

</script>

<div class="cacheConfigContainer">
    <div class='cacheConfigTextContainer'>
        <h3>
            Configuring your cache
        </h3>
        <div>
            <p>
                Configuring your custom cache couldn't be easier. You have the option to input your cache type, cache capacity, and the expiration time or use default values. 
                <br>
                <br>
                If you're a Redis fan, we've got integration for that too. Simply input Redis as your cache type and select your port number.
            </p>
        </div>
    </div>

    <div class='cacheConfigImgContainer'>
        <img id='cacheOptionsScreenshot' src='../public/images/cacheOptions.png' alt='sample code of a user initiating a Zoic cache object'>
    </div>
</div>

<style>
    .cacheConfigContainer {
        color: white;
        display: flex;
        justify-content: space-around;

    }

    .cacheConfigTextContainer {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* background-color: #E76020; */
        padding: 20px;
        text-shadow: 2px 2px #ff0000;
    }

    #cacheOptionsScreenshot {
        width: 80%;
        height: 80%;
        padding: 10px;
        box-shadow: 5px 10px 18px #888888;
        border-radius: 7%;
    }

    .cacheConfigImgContainer {
        width: 80%;
        height: 80%;
        /* background-color: #E76020; */
        padding: 20px;
        display: flex;
        justify-content: center;
    }


</style>