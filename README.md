# nuxt-setel
**It can't do much, but it's okay**
Super easy Text-Editor light for Nuxt.js using Vue.js

# Super light
**Most TextEditors are overperforming**
In my cases, 90% of times when I need a HTML Text Editor I just need to:
 - Bold text 
 - Italic text 
 - Underline text 
 - Justify text center
 - Justify text left
 - brakes and spaces

This Texteditor only provides these, while easy to include and adapt via two components
One for the HTML TextEditor itself
One for the ActionBar like bold and justify buttons which you can place wherever you like.

# Super easy to include
No need to install or merge this file to your existing project.
Just download the two components in this Repo,

Paste them to your components directory and include them in your script

    import TextEditor from '~/components/TextEditor.vue'
	import TextEditorActions from '~/components/TextEditorActions.vue'
	...
	export default {
		components: {
		    TextEditor,
		    TextEditorActions
		  },
	  }
	  ...

Include the two components page/section where you want the TextEditor and his ActionsBar to be.

    // The ActionBar like justifying the text or bold
    <TextEditorActions />

    // The HTML TextEditor itself
    <TextEditor
      v-model="ProjectDescription"
      style="min-height:320px"
    ></TextEditor>

# Super easy to understand
**Even your Dad would understand this, at least he pretends to**
Just two Vue.js components with super easy to understand html and Vue.js script,
which need to be included where you want the TextEditor to be.
Bind the TextEditor with [v-model](https://vuejs.org/v2/guide/forms.html) and you are set.

# Super easy to extend
If you want to add more functions to the ActionBar just add buttons with the specific function
You can look up the possibilities here:
 [TextEditorActions](https://reference.codeproject.com/book/dom/document/execcommand)
You can add styling to the TextEditor easily in the component itself 
and place the ActionBar wherever you like even multiple TextEditors in one page.


 
