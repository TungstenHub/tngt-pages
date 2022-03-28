**Axiom of Extensionality (AEx)**

$$\forall x \forall y (\forall z(z\in x\longleftrightarrow z\in y)\longrightarrow x=y)$$

**Axiom of Empty Set (AEm)**

$$\exists x\forall y \neg(y\in x)$$

**Axiom-Schema of Specification (ASp)**

$$\forall y_1...\forall y_n (\forall z\exists y\forall x(x \in y \longleftrightarrow x \in z \wedge \varphi(x; y_1 ,..., y_n )))$$

**Axiom of Pairing (APr)**

$$\forall x\forall y\exists z\forall u(u \in z \longleftrightarrow u = x \vee u = y)$$

**Axiom of Union (AUn)**

$$\forall x\exists y\forall z(z \in y \longleftrightarrow \exists u(u \in x \wedge z \in u))$$

**Axiom of Power Set (APw)**

$$\forall x\exists y\forall z(z \in y \longleftrightarrow \forall u(u \in z \longrightarrow u \in x))$$

**Axiom of Infinity (AIn)**

$$\exists y(\exists z(z \in y \wedge \forall t\neg (t \in z)) \wedge \forall x(x \in y \longrightarrow \exists u(u \in y \wedge \forall v(v \in u \longleftrightarrow v = x \vee v \in x)))$$

**Axiom-Schema of Replacement (ARep)**

$$\forall y_1...\forall y_n [\forall x\forall y\forall y' (\varphi(x, y; y_1 ,..., y_n ) \wedge \varphi(x, y' ; y_1 ,..., y_n ) \longrightarrow y= y' ) \\ 
\longrightarrow \forall u\exists v\forall z(z \in v \longleftrightarrow \exists w(w \in u \wedge \varphi(w, z; y_1 ,..., y_n )))]$$

**Axiom of Choice (AC)**

$$\forall x \exists f (f \text{ is a function} \wedge \forall y (y \in x \wedge y \neq \varnothing \longrightarrow f (y) \in y))$$

**Axiom of Regularity (AReg)**

$$\forall x(\exists y(y \in x) \longrightarrow \exists z(z \in x \wedge \forall u\neg (u \in z \wedge u \in x))$$