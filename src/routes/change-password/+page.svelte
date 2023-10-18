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
    <h4 style="text-align: center"> 비밀번호 변경 </h4>
    <Textfield
            style="width: 240px;"
            label="이전 비밀번호"
            bind:value={beforePassword}/>
    <Textfield
            style="width: 240px;"
            label="새로운 비밀번호"
            bind:value={newPassword}/>
    <Textfield
            style="width: 240px;"
            label="비밀번호 확인"
            bind:value={newPasswordConfirm}/>
    <Button style="width: 280px; margin-top: 1vh" color="primary" variant="raised" on:click={sendData}>
        <Label>CHANGE PASSWORD</Label>
    </Button>
</div>

<style>
    .form-container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 80vh;
        flex-direction: column;
    }
</style>