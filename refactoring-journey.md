1. Comment out all ruby script blocks via following command
    :g/ruby << EOF/,/EOF/s/^/"
2. Comment out all ruby command calls via following command
    :g/^\sruby/s/^/"
3. Add 'TODO ruby code' as comment above each ruby code segment
    g/^"\s*ruby \(<< EOF\)\{0,1}/-pu =\"\\"TODO ruby code\"

