<script>
    import Textfield from "@smui/textfield";
    import Card from "@smui/card";
    import Button, {Label} from "@smui/button";
    import axios from "axios";
    import {goto} from "$app/navigation";

    let beforePassword = "";
    let newPassword = "";
    let newPasswordConfirm = "";

    const sendData = () => {
        const requestData = {
            password: newPassword,
            passwordConfirm: newPasswordConfirm
        };
    }
</script>


<div class="form-container">
    <Card>
        <h2 style="text-align: center"> 비밀번호 변경 </h2>
        <Textfield
                label="BEFORE_PASSWORD"
                bind:value={beforePassword}/>
        <Textfield
                label="NEW_PASSWORD"
                bind:value={newPassword}/>
        <Textfield
                label="PASSWORD_CONFIRM"
                bind:value={newPasswordConfirm}/>
        <Button color="primary" variant="raised" on:click={sendData}>
            <Label>LOGIN</Label>
        </Button>
    </Card>
</div>

<style>
    .form-container {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 80vh;

    }
</style>