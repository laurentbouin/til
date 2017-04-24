### Parse logback logs through Filebeat

In order to append stacktrace lines to the previous message you have to define a multiline pattern. 
For Filebeat this pattern is: 

``` shell
  # The regexp Pattern that has to be matched. 
  multiline.pattern: '^[[:digit:]]{4}-[[:digit:]]{2}-[[:digit:]]{2}'
  
  # Defines if the pattern set under pattern should be negated or not. Default is false.
  multiline.negate: true

  # Match can be set to "after" or "before". It is used to define if lines should be append to a pattern
  # that was (not) matched before or after or as long as a pattern is not matched based on negate.
  multiline.match: after

```