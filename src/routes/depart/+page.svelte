<script lang="ts">
    import Card from "@smui/card";
</script>

<h1>학과 목록</h1>

<div class="card-display">
    <div class="card-container">
        <Card color="secondary" variant="raised" padded>경영</Card>
    </div>
    <div class="card-container">
        <Card color="secondary" variant="raised" padded>컴공</Card>
    </div>
    <div class="card-container">
        <Card color="secondary" variant="raised" padded>겜공</Card>
    </div>
</div>


<style>
    .card-display {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 70vh;
        flex-direction: row;
        flex-wrap: wrap;
        align-content: space-around;
    }

    .card-container {
        height: 20vw;
        width: 18vw;
    }
</style>