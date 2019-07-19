<template>
  <section class="section">
    <form
      name="contact"
      method="POST"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
    >
    <input type="hidden" name="form-name" value="contact" />
    <input type="hidden" name="bot-field" />

      <div className="form-group">
        <label>お名前<abbr title="required">*</abbr>
        <input type="text" className="form-control" id="name" name="name" placeholder="お名前" maxlength="30" minlength="2" required autocomplete="name" />
        </label>
      </div>
      <div className="form-group">
        <label>メールアドレス<abbr title="required">*</abbr>
        <input type="email" className="form-control" id="email" name="email" placeholder="" pattern="^[a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$" required autocomplete="email" />
        </label>
      </div>
      <div className="form-group">
        <label>お問い合わせ内容<abbr title="required">*</abbr>
        <textarea className="form-control" id="contact" name="content" rows="8" required></textarea>
        </label>
      </div>

      <div className="form-group">
      <button type="submit">送信</button>
      </div>
    </form>
    <div class="columns is-mobile">
      <card
        title="Free"
        icon="github-circle"
      >
        Open source on <a href="https://github.com/buefy/buefy">
          GitHub
        </a>
      </card>

      <card
        title="Responsive"
        icon="cellphone-link"
      >
        <b class="has-text-grey">
          Every
        </b> component is responsive
      </card>

      <card
        title="Modern"
        icon="alert-decagram"
      >
        Built with <a href="https://vuejs.org/">
          Vue.js
        </a> and <a href="http://bulma.io/">
          Bulma
        </a>
      </card>

      <card
        title="Lightweight"
        icon="arrange-bring-to-front"
      >
        No other internal dependency
      </card>
    </div>
  </section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',

  components: {
    Card
  }
}
</script>
