Trie.js
=======

A Trie in Javascript

This fork enables a new method: collapse()
Collapsing a trie converts its elements into a shell-style expansion string

A convenience method exists exposing just this functionality using a throwaway object:

    let trie = new Trie;
    console.log('Collapsed trie is: "' + trie.collapseFromArray(['spill', 'spall', 'spell']) + '"');
    // "sp{ill,all,ell}"

This behavior should mirror Bash's reverse completion 'complete-into-braces' readline command, activated interactively using Meta + { (typically Alt + Left-Curly)
