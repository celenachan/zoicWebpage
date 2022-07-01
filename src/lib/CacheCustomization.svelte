<script>

</script>

<div class="cacheConfigContainer">
    <div class='cacheConfigTextContainer'>
        <h3>
            Configuring your cache
        </h3>
        <div>
            <p>
                Configuring your custom cache couldn't be easier. You have the option to input your cache type, cache capcity, and the expiration time or use default values. 
                <br>
                <br>
                If you're a Redis fan, we've got integration for that too. Simply input Redis as your cache type and select your port number.
            </p>
        </div>
    </div>

    <div class='cacheConfigImgContainer'>
        <img src='../public/images/cacheOptions.png' alt='sample code of a user initiating a Zoic cache object'>
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
        background-color: purple;
        padding: 20px;
    }

    .cacheConfigImgContainer {
            background-color: white;
    }


</style>