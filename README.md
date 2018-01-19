# Emerald: HTML 5 Templating Engine for Nim

This is a fork which fixes a compatibility issue with Nim 0.17.2. The only change so far is that the form method attribute couldn't be properly escaped without causing a keyword conflict, so a workaround was devised whereby the method attribute was _internally_ named formmethod to avoid this conflict. However, you can still use the normal

    form(`method`="post", ...): ...
    
template.

Documentation:

http://flyx.github.io/emerald/
