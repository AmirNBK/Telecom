<script>
    import image from "../../assets/image/ContactUsImage.png";
  
    const locations = [
      { title: "Europe", countries: ["Telecom Easy", "Telecom Scandinavia", "Telecom Easy Sca"] },
      { title: "Africa", countries: ["Telecom Easy", "Telecom Scandinavia", "Telecom Easy Sca"] },
      { title: "Asia", countries: ["Telecom Easy", "Telecom Scandinavia", "Telecom Easy Sca"] }
    ];
  </script>
  
  <div class="ContactUsContainer rounded-md pb-8" style="box-shadow: 0px 4px 80px 0px rgba(0, 0, 0, 0.10);">
    <h2 style="background-color: #0E3552;" class="text-xl rounded-t-md text-white px-4 py-2">
      contact us
    </h2>
    <img src={image} alt="image" class="ml-4 rounded-md mt-4 w-8/12" />
  
    {#each locations as location}
      <div class="ml-4 mt-3">
        <h2 style="color: #DC0600;" class="text-2xl mb-2">{location.title}</h2>
        {#each location.countries as country}
          <p class="text-xl">{country}</p>
        {/each}
      </div>
    {/each}
  </div>
  