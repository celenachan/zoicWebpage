<script>
    import CodeBlockCustom from "./CodeBlockCustom.svelte";
</script>

<div class="cacheConfigContainer">
    <div class='cacheConfigTextContainer'>
      <div class="cacheConfigTitle">
            <i>
                Configuring your cache
            </i>
      </div>
        <div>
            <p>
                Configuring your custom cache couldn't be easier. You have the option to input your cache type, cache capacity, and the expiration time or use our pre-selected default values. 
                <br>
                <br>
                If you're a Redis fan, we've got integration for that too. Simply input Redis as your cache type and select your port number.
            </p>
        </div>
    </div>

    <div class='cacheConfigImgContainer'>
        <CodeBlockCustom />
    </div>
</div>

<style>
    .cacheConfigContainer {
        color: white;
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        align-items: center;
        font-size: 1.4rem;
    }



    .cacheConfigTextContainer {
        display: flex;
        flex-direction: column;
        width: 575px; 
        margin: 15px;
      }
      
      .cacheConfigTitle {
        font-size: 2.3em;
        text-shadow: 2px 2px 4px;
    }

    #cacheOptionsScreenshot {
        /* padding: 15px;
        box-shadow: 5px 10px 18px #888888;
        border-radius: 7%;
        width: 580px; */
        /* min-width: 300px;
        min-height: 160px; */
        margin: auto;
        border-radius: 30px;
        border: 2px solid rgb(53, 47, 47);
        box-shadow: 10px 5px 5px rgb(127, 124, 124);

    }

    .cacheConfigImgContainer {
        width: 50%;
        height: 90%;
        padding: 20px;
        display: flex;
        justify-content: center;
    
    }

    p {
    color: white;
    font-size: 1.5rem;
    }

  @media screen and (max-width: 800px) {
    .cacheConfigTextContainer {
    text-align: center;
  }
}

   

</style>