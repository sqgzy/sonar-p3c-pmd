# ShortInstantiation
**Category:** `pmd`<br/>
**Rule Key:** `pmd:ShortInstantiation`<br/>


-----

In JDK 1.5, calling new Short() causes memory allocation. Short.valueOf() is more memory friendly.  Example :
<pre>
public class Foo {
private Short i = new Short(0); // change to Short i =
Short.valueOf(0);
}
  </pre>
