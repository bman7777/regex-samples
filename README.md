# regex-samples

## Remove something from the start of the match OR accept all that don't match (and trim off everything after colon.)
`((?!^registry\.)|(^registry\.\Kin\.thewardro\.be)).+(?=:)`

input => registry.in.thewardro.be/dshfkjdhfkjd:47589  output=>   in.thewardro.be/dshfkjdhfkjd
input => ruby.foo.bar/fkjds:47589  output=>   ruby.foo.bar/fkjds
