# rna
RNA gene drawing
```
phe_seq = 'GCGGAUUUAGCUCAGUUGGGAGAGCGCCAGACUGAAGAUCUGGAGGUCCUGUGUUCGAUCCACAGAAUUCGCACCA';
phe_str = rnafold(phe_seq);

% === Plot RNA secondary structure as tree
rnaplot(phe_str, 'seq', phe_seq, 'format', 'tree');
% === Plot the secondary structure using the dot diagram representation
rnaplot(phe_str, 'seq', phe_seq, 'format', 'dot');

text(500, 200, 'T-stem');
text(100, 600, 'Anticodon stem');
text(550, 650, 'D-stem stem');
text(700, 400, 'Acceptor stem');
aag_pos = 34:36;
cca_pos = 74:76;
rnaplot(phe_str, 'sequence', phe_seq, 'format', 'diagram', ...
    'selection', [aag_pos, cca_pos]);
```



![](https://github.com/iostreamatlab/rna/raw/master/rna-1.jpg)  

