hello-world
===========

Juste pour essayer.

Bien, à présent, je fais une modification. Et puis, j'écris des trucs depuis mon Gros Ordi.
Mais, maintenant, j'écris sur le vaibe. C'est dingue.

Un peu de code _scala_:

```scala
package euler1

object Utils {
  def factoriel(n: Int): Int = {
                  def facHelper(m: Int, accum: Int): Int =
      if (m == 0) accum else facHelper(m - 1, accum * m)
    facHelper(n, 1)
  }

  def diviseurs(n: Int): List[Int] =
    if (n > 0)
      1 :: (for (d <- (2 to n / 2); if (n % d == 0)) yield d).toList
    else
      throw new Error("Utils.diviseurs appelé pour nombre inférieur à 1")

  def sommeDiviseurs(n: Int): Int = diviseurs(n) reduce (_ + _)

  def amicaux(n1: Int, n2: Int): Boolean =
    sommeDiviseurs(n1) == n2 && sommeDiviseurs(n2) == n1

}
```

Et un truc _ruby_:

```ruby
def afficheNum
   # p $piles
   ($n-1).downto(0) { |etage|
      1.upto(3) { |pile|
         print("  " + ($piles[pile][etage] || "|").to_s)
      }
      print("\n")
   }
   print("-----------\n\n")
end
```

Et une liste:
* truc
* machin
* chose
* 

Peut-on faire du LaTex ?
$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

