<script lang="ts">
  import IconButton from '@smui/icon-button';
  import Paper, { Content } from '@smui/paper';
  import TopAppBar, { Row, Section, Title } from '@smui/top-app-bar';

  export let name: string;
</script>

<main>
  <TopAppBar variant="static">
    <Row>
      <Section>
        <IconButton class="material-icons">menu</IconButton>
        <Title>Hello {name}!</Title>
      </Section>
    </Row>
  </TopAppBar>
  <div>
    <Paper>
      <Content
        >Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn
        how to build Svelte apps.</Content
      >
    </Paper>
  </div>
  <div>
    <Paper>
      <Content
        >Visit <a href="https://sveltematerialui.com">Svelte Material UI</a> to learn
        how to use SMUI components.</Content
      >
    </Paper>
  </div>
</main>

<style>
  :global(body, html) {
    height: 100%;
    margin: 0;
    padding: 0;
  }

  div {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }
</style>
