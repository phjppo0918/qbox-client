<script>
    import Button, {Label} from "@smui/button";

    import TopAppBar, {
        Row,
        Section,
        Title,
        AutoAdjust,
    } from '@smui/top-app-bar';

    let topAppBar;
</script>



<TopAppBar color="secondary" bind:this={topAppBar} variant="short">
    <Row>
        <Section>
            <Title>QBOX</Title>
        </Section>
        <Section align="end">
            <Button href="/signup" variant="raised">
                <Label>sign up</Label>
            </Button>
            <Button href="/login" variant="outlined">
                <Label>login</Label>
            </Button>
        </Section>
    </Row>
</TopAppBar>
<AutoAdjust {topAppBar}/>