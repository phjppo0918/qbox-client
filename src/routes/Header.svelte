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
            <Button variant="raised">
                <Label>signup</Label>
            </Button>
            <Button color="primary" variant="outlined">
                <Label>signin</Label>
            </Button>
        </Section>
    </Row>
</TopAppBar>