<script>
    import Textfield from "@smui/textfield";
    import Card from "@smui/card";
    import Button, {Label} from "@smui/button";

</script>
<form method="post" class="login-container">
    <Card>
        <h2 style="text-align: center"> 회원가입 </h2>
        <Textfield
                label="EMAIL"
                value=""
                input$name="email"/>
        <Textfield
                label="NICKNAME"
                value=""
                input$name="nickname"/>
        <Button color="primary" variant="raised">
            <Label>SIGN UP</Label>
        </Button>
    </Card>
</form>

<style>
    .login-container {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 80vh;
    }
</style>