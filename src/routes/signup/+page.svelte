<script>
    import Textfield from "@smui/textfield";
    import Card from "@smui/card";
    import Button, {Label} from "@smui/button";
    import {goto} from '$app/navigation';
    import axios from "axios";

    var email = ""
    var nickname = ""

    const sendData = () => {
        const requestData = {
            email,
            nickname
        };

        axios({
            method: "post",
            url: "members",
            data: requestData
        }).then(() => goto("/signup/fin"));

    }
</script>
<div class="signup-container">
    <Card>
        <h2 style="text-align: center"> SIGN UP </h2>
        <Textfield
                label="EMAIL"
                bind:value={email}/>
        <Textfield
                label="NICKNAME"
                bind:value={nickname}/>
        <Button color="primary" variant="raised" on:click={sendData}>
            <Label>NEXT</Label>
        </Button>
    </Card>
</div>

<style>
    .signup-container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 80vh;
        flex-direction: column;
    }
</style>