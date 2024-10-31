### "Google" "Blockly" "Prototypes"

This repository contains obfuscated Python code masquerading as something vaguely equivalent to Scratch (Blockly graphs). 

Based on the sheer quantity of nodes in these graphs, this code was almost certainly originally written in python and converted to this utterly unhinged format by tooling which the author will no doubt never admit to the existence of, rather than being created by hand in a blockly/scratch editor.

Further evidence of this comes from the... let's be nice and say "novel embedded runtime", which mostly just executes a series of (violently insecure) eval() calls and string replacements to clunkily and inefficiently rehydrate the original python code (some segments of which can be found in strings within the enormous dict-that-could've-been-a-JSON-if-you-really-had-to-do-it at the top of each file), rather than the graph having been used to generate sane if rather verbose python code (which is what even the basic Blockly example python code generator does)

One assumes the intent is to prevent users from determining the provenance of any code such obfuscated, enabling the author to continue their habit of copying code from other open source repositories without attribution (and denying having done so, despite incontrovertible evidence of this unethical, egotistical, community-hostile behaviour) while preventing anyone from calling them out for it.
