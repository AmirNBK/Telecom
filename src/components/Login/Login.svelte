<script>
    import image from "../../assets/image/loginImage.png";
    import LoginInputs from "../LoginInputs/LoginInputs.svelte";
    import user from "../../assets/icons/user.svg";
    import phone from "../../assets/icons/phone.svg";
    import email from "../../assets/icons/email.svg";
    import chat from "../../assets/icons/chat.svg";
</script>

<div
    class="LoginContainer rounded-md pb-8"
    style="box-shadow: 0px 4px 80px 0px rgba(0, 0, 0, 0.10);"
>
    <h2
        style="background-color: #0E3552;"
        class="text-xl rounded-t-md text-white px-4 py-2"
    >
        Login
    </h2>
    <img src={image} alt="image" class="ml-4 rounded-md mt-4 w-8/12" />

    <div class="LoginContainer__infos ml-4 mt-8">
        <p class="text-3xl">03054886</p>
        <p class="text-xl my-6">BSC 32UMPTb2_WD2DOUMPTB02 NEW</p>

        <div class="flex flex-col gap-6">
            <LoginInputs text="Name" icon={user} />
            <LoginInputs text="Your phone" icon={phone} />
            <LoginInputs text="Your email address" icon={email} />
            <div class="flex items-baseline gap-32">
                <LoginInputs text="comment" icon={chat} />
                <button
                    class="rounded-md py-2 px-6 w-fit text-sm mt-2 text-white"
                    style="background : #9C1511"
                    >send request for Quotation</button
                >
            </div>
        </div>
    </div>
</div>
