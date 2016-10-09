# n
// client/commonFramework/create-editor.js

window.common = (function(global) {
  // ...
  common.init.push(function() {
    // ...
    editor.setValue(common.replaceSafeTags(editorValue));
    editor.getDoc().clearHistory(); // add this line
    editor.refresh();
  });
  // ...
}(window));
