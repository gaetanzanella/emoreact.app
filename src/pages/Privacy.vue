<template>
  <Layout>
    <div class="container">

      <div class="contact-header">
        <h1 class="contact-title">Privacy policy</h1>
        <p>Emoreact' cares about privacy. You can use the app whithout exposing any personnal data.</p><p>This page informs visitors regarding the Emoreact' policies with the collection, use, and disclosure of personal content in case you consent to give to Emoreact' access to some of your personal data.</p>
        <h3>Data Collection and Use</h3>
        <p>Emoreact' does not require access to any user data to be functionnal. Nevertheless it may request an access to your photo library and your camera if you wish to create custom reactions or search reactions using your face.<p>
        <p>When creating a reaction from your photo library, only the content you select is exposed to Emoreact'. It does not have access to your entire library.</p>
        <p>When searching reactions using your face, Emoreact' uses the TrueDepth technology of your camera to deternime your current facial expression. Face recognition and search is done completely on your device.</p>
        <h3>Data Storage</h3>
          <p>Personal content (such as custom reactions) is not saved on our servers nor do we have access to this data. This data is saved locally on your devices and, in case you are using the iCloud function of the application, synchronized with your personal iCloud CloudKit database (Apple service). It allows you to keep your Emoreact' data synchronized between your devices and prevents data loss. You always have the option to disable iCloud or delete your iCloud data from the system settings.</p>
        <h3>Third parties</h3>
          <p>Emoreact' does not use analytics tools, advertising networks or third-party SDKs. It does not share your data with external entities.</p>
          <p>Nevertheless you may yourself expose some of your data if you use the reaction sharing feature. In such case, you expose the shared data to any Emoreact' user who has the sharing iCloud link. Be sure to share your data consciously. Emoreact' still does not access to this data.</p>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {}
</script>

<style scoped>
.contact-header {
  padding: 2rem 0 4rem 0;
}
.contact-title {
  font-size: 4rem;
  margin: 0 0 4rem 0;
  padding: 0;
}
.sender-info {
  display: flex;
  flex-wrap: wrap;
  margin-bottom: 2rem;
}
.sender-info > div {
  flex: 1;
  margin-right: 4rem;
}
.sender-info > div:last-of-type {
  margin: 0;
}
input:focus,textarea:focus {
  border-color: var(--color-contrast-1);
}
input,textarea {
  background: transparent;
  border: 1px solid var(--color-base-1);
  outline: none;
  border-radius: 0.3rem;
  padding: 0.8rem 1rem;
  color: inherit;
  font-size: 1rem;
  width: 100%;
}
textarea {
  resize: none;
  height: 140px;
}
.button {
  color: var(--color-base);
  background: var(--color-contrast);
  outline: none;
  border: 0;
  font-size: 0.8rem;
  padding: 0.8rem 1.6rem;
  border-radius: 0.3rem;
  margin-top: 2rem;
  cursor: pointer;
  transition: opacity 0.25s ease;
  font-size: 500;
  letter-spacing: 0.035em;
}
.button:hover {
  opacity: 0.6;
}
.button:focus {
  border: 1px solid var(--color-base-1);
}
</style>

