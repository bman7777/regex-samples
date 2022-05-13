# regex-samples

## Remove something from the start of the match OR accept all that don't match (and trim off everything after colon.)
`((?!^registry\.)|(^registry\.\Kin\.thewardro\.be)).+(?=:)`

| input | output |
| ----- | ------ |
| registry.in.thewardro.be/dshfkjdhfkjd:47589 | in.thewardro.be/dshfkjdhfkjd |
| ruby.foo.bar/fkjds:47589 | ruby.foo.bar/fkjds |
