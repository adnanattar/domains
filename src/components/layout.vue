<script setup>
const TWITTER_HANDLE = "web3shiftweb";
const TWITTER_LINK = `https://twitter.com/${TWITTER_HANDLE}`;
</script>
<template>
  <div className="App">
    <div className="container">
      <div className="header-container">
        <header>
          <div className="left">
            <p className="title">Web3Shift Name Service</p>
            <p className="subtitle">For a stronger web identity</p>
          </div>
        </header>
      </div>
      <slot></slot>

      <div className="footer-container">
        <img
          alt="Twitter Logo"
          className="twitter-logo"
          src="/twitter-logo.svg"
        />
        <a
          className="footer-text"
          :href="TWITTER_LINK"
          target="_blank"
          rel="noreferrer"
          >{{ `built with @${TWITTER_HANDLE}` }}</a
        >
      </div>
    </div>
  </div>
</template>
