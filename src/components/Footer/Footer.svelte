<script>
    import facebook from "../../assets/icons/facebook.svg";
    import linkedin from "../../assets/icons/linkedin.svg";
    import wifi from "../../assets/icons/wifi.svg";
</script>

<div class="Footer" style="background-color: #064973;">
    <div
        class="px-6 text-white flex flex-row justify-around pt-6 flex-wrap mt-10 gap-12 md:gap-2"
    >
        <div class="Footer__leftside gap-4 flex flex-col">
            <div class="Footer__leftside_info">
                <h4 class="text-2xl mb-1">Information</h4>
                <a href="/">Home</a> <br/>
                <a href="/products">Products</a> <br/>
                <a href="/about-us"> About us </a> <br/>
                <a href="/contact-us">Contact us</a>
            </div>
        </div>

        <div class="Footer__centerside">
            <div class="Footer__centerside__company">
                <h4 class="text-2xl mb-1">Company</h4>
                <a href="/about-us">Our team</a>
                <br/>
                <a href="contact-us">Contact us</a>
            </div>
        </div>

        <div class="Footer__rightside">
            <div class="Footer__rightside__service">
                <h4 class="text-2xl mb-1">Customer service</h4>
                <a href="/">Home</a> <br/>
                <a href="/news">News</a> <br/>
                <a href="/products">Products</a> 
            </div>
        </div>

        <div class="Footer__newsLetter">
            <h4 class="text-2xl">Newsletter</h4>
            <div
                class="Footer__newsLetter__subscribe flex flex-col justify-between"
            >
                <h4 class="text-black">Newsletter</h4>
                <div class="flex flex-col items-end">
                    <input
                        placeholder="Enter your email here..."
                        class="mt-1 mb-3 outline-none text-black px-5 py-3 rounded-md"
                    />
                    <button
                        style="background-color: #CECECEEB;"
                        class="rounded-md px-2 py-1 ml-2">Subscribe</button
                    >
                </div>
            </div>

            <div class="Footer__newsLetter__socialMedia">
                <h4 class="text-2xl">Follow us</h4>
                <div class="flex flex-row gap-2 items-baseline">
                    <img
                        src={facebook}
                        class="w-5 h-10"
                        alt="Social Media Icons"
                    />
                    <img
                        src={linkedin}
                        class="w-5 h-10"
                        alt="Social Media Icons"
                    />
                    <img
                        src={wifi}
                        class="w-8 h-8"
                        alt="Social Media Icons"
                        style="transform: translateY(-2px);"
                    />
                </div>
            </div>
        </div>
    </div>

    <div class="w-full h-14 mt-6" style="background-color: #0E3552;" />
</div>
