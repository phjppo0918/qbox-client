<script>
    import Textfield from "@smui/textfield";
    import Card from "@smui/card";
    import Button, {Label} from "@smui/button";
    import axios from "axios";
    import {goto} from "$app/navigation";

    let email = "";
    let password = "";

    const sendData = () => {
        const requestData = {
            email,
            password
        };

        axios({
            method: "post",
            url: "login",
            data: requestData,
            headers: {
                "Content-Type": "multipart/form-data",
            },
        }).then(() => goto("/", {replaceState: true}));
    }
</script>


<div class="login-container">
    <h4 style="text-align: center"> LOGIN </h4>
    <Textfield
            label="EMAIL"
            bind:value={email}/>
    <Textfield
            label="PASSWORD"
            bind:value={password}/>
    <Button style="width: 180px; margin-top: 1vh" color="primary" variant="raised" on:click={sendData}>
        <Label>LOGIN</Label>
    </Button>
</div>

<style>
    .login-container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 80vh;
        flex-direction: column;
    }
</style>