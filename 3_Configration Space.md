# 3 Conﬁguration Space

TO CREATE motion plans for robots, we must be able to specify the position of the robot. More speciﬁcally, we must be able to give a speciﬁcation of the location of every point on the robot, since we need to ensure that no point on the robot collides with an obstacle.
This raises some fundamental questions: How much information is required to completely specify the position of every point on the robot? How should this information be represented? What are the mathematical properties of these representations? How can obstacles in the robot’s world be taken into consideration while planning the path of a robot?In this chapter, we begin to address these questions.
We ﬁrst discuss exactly what is meant by a conﬁguration of a robot and introduce the concept of the conﬁguration space, one of the most important concepts in robot motion planning.
We then brieﬂy discuss how obstacles in the robot’s environment restrict the set of admissible paths. 
We then begin a more rigorous investigation of the properties of the conﬁguration space, including its dimension, how it sometimes can be represented by a differentiable manifold, and how manifolds can be represented by embeddings and parameterizations.
We conclude the chapter by discussing mappings between different representations of the conﬁguration, and the Jacobian of these mappings, which relates velocities in the different representations.

(Google翻訳)
ロボットの動作計画を作成するには、ロボットの位置を指定できる必要があります。
より具体的には、ロボット上のどの点も障害物に衝突しないようにする必要があるため、ロボット上のすべての点の位置の指定が可能でなければなりません。
これはいくつかの根本的な疑問を提起します：ロボットのあらゆる点の位置を完全に指定するためにはどのくらいの情報が必要ですか？この情報はどのように表現されるべきですか？これらの表現の数学的性質は何ですか？ロボットの進路を計画する際に、ロボット世界の障害をどのように考慮に入れることができますか？
この章では、これらの問題に取り組み始めます。
最初に、ロボットの構成が何を意味しているかを正確に議論し、ロボット運動計画の最も重要な概念の1つである構成空間の概念を導入する。
次に、ロボット環境内の障害物がどのように許容経路の集合を制限するかについて簡単に議論する。
次に、構成空間の特性、その次元、時には微分可能な多様体によって表現される方法、および多様体が埋め込みとパラメータ化によってどのように表現されるかという、より厳密な調査を開始する。
この章では、構成の異なる表現と、異なる表現の速度に関係するこれらのマッピングのヤコビ行列との間のマッピングについて論じることで、結論を述べる。


