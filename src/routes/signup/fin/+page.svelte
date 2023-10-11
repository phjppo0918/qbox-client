<script>
    import Button, {Label} from "@smui/button";
    import {goto} from "$app/navigation";

</script>

<h2>입력한 이메일로 임시 비밀번호가 갔어요. 로그인 이후에 비밀번호를 변경해주세요</h2>
<Button on:click={() => goto("/")}>
    <Label>메인페이지로</Label>
</Button>
