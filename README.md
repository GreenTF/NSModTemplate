# NSModTemplate
A template repository for Northstar mods with a ~~mostly~~ pre-configured github action for publishing to Thunderstore

## Usage
<ol>
<li> Click the <code>Use this template</code> button on the top right of the repo's landing page (<a href="https://github.com/GreenTF/NSModTemplate">here</a>)</li>
<li> Give the new repo a name and make sure it's set to <code>public</code></li>
<li> <details><summary> In the <code>settings</code> tab, under <code>actions</code> -> <code>general</code>, set <code>Actions permissions</code> to <code>Allow all actions and reusable workflows</code></summary>
<img src="https://user-images.githubusercontent.com/4367791/180306016-04bfc321-b60f-4ed0-ac0c-5a6065036e2c.png" />
</details></li>
<li> <details><summary> Also in <code>settings</code>, under <code>secrets</code> ->  <code>actions</code>, add your Thunderstore token as a secret named <code>TS_KEY</code> (Steps for getting a token can be found <a href="https://github.com/GreenTF/upload-thunderstore-package/wiki">here</a>)</summary>
  <img src="https://user-images.githubusercontent.com/4367791/180306285-60dd51ec-0448-44af-aa92-682599c6c0f4.png" />
  <img src="https://user-images.githubusercontent.com/4367791/180306391-a217f309-e875-4e74-8270-8155c60dbcdc.png" />
</details>
</li>
  <li> <details><summary>Edit <code>.github/workflows/publish.yml</code> ~line 43 to add a description for your mod </summary>
    <img src="https://user-images.githubusercontent.com/4367791/180337843-5213db45-850b-4759-98c5-9ad47cbab7ba.png" />
    </details>
  </li>

<li> Update this README and <code>icon.png</code> as they will be used by Thunderstore as well </li>
<li> Write your mod! (HINT: Find the docs <a href="https://r2northstar.readthedocs.io/en/latest/guides/gettingstarted.html">here</a>) </li>
<li> <details><summary>Publish your mod!</summary>
  Once you've pushed all your chages to your repo, you'll need to create a tag to trigger the action that will publish your mod to Thunderstore.
  Find the `Releases` pane in the sidebar to the right ---->
  <br />
  <img src="https://github.com/GreenTF/NSModTemplate/assets/4367791/cd789d16-dd0a-4310-8dc1-c1781b6c66a8" />
  <br />
  Create a new release, filling in the details however you want. The most important part is that the tag matches the version number of your mod. In this example, the <code>Version</code> field in your <code>mod.json</code> should be <code>1.0.0</code>:
  <br />
  <img src="https://github.com/GreenTF/NSModTemplate/assets/4367791/e3fd6bad-4d1c-438c-b3a3-b683c1316ab5" />
  <br />
  Once you've added a title and optional description, go ahead and publish that release.
  <br />
  <img src="https://github.com/GreenTF/NSModTemplate/assets/4367791/9da50c60-87f1-40aa-b5a9-9c69becd4026" />
  <br />
  If all goes well, you should see a new publish job running in the <code>Actions</code> tab :D
</details>
</li>
</ol>


