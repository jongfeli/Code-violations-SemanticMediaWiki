# Code-violations-SemanticMediaWiki

[Fix coding style issues #899](https://github.com/SemanticMediaWiki/SemanticMediaWiki/issues/899)

[syncing-a-fork](https://help.github.com/articles/syncing-a-fork/)

```php
  if ( some condition ) {
    doSomeStuff
    }

	/**
	 * We use the internal wikipage object to store some of this objects data.
	 * Clone it to make sure that data can be modified independently from the
	 * original object's content.
	*/
	public function __clone() {
		if ( !is_null( $this->m_wikipage ) ) {
			$this->m_wikipage = clone $this->m_wikipage;
		}
	}
	
	if ( $subCondition instanceof FalseCondition ) {
      return new FalseCondition();
  } // @codingStandardsIgnoreStartphpcs, ignore --sniffs=.....
  elseif ( $subCondition instanceof TrueCondition ) {
        // ignore true conditions in a conjunction
  } // @codingStandardsIgnoreEnd
```
