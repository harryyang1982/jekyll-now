---
id: 3348
title: 대통령 선거에서 테크놀로지의 역할(The Economist, Nov 20, 2016)
date: 2016-11-26T23:24:46+00:00
author: 양승훈
layout: post
comments: true
---
**예측 모델링과 클러스터링에 따른 개인화 등을 활용한 데이터 과학을, 짝퉁 뉴스(fake news)와 반향실(echo chamber)에서 맴맴도는 확산의 소셜미디어가 이겼다.** 소셜 미디어에서 &#8216;어그로&#8217;를 끌며 계속 반쪽짜리 사실과 거짓말을 구태여 부정하지 않은 트럼프의 트위터 메시지가 이겼다는 거다. 온갖 종류의 &#8216;올바르지 않은 막말&#8217;을 구현했지만, 어쨌든 트럼프가 더 많은 메시지를 증폭시켰기 때문이다. (역설적으로 한국에서는 페이스북 사용이나 구글 사용이 적어, 미국 같은 결과가 나오지는 않을 거라는 생각도 든다. 필터 버블이라는 베이즈 통계 기반보다는, 한국에서는 맞춤형 대신 전체 통계로 랭킹을 보여주는 것이 여전히 보편적이므로.. 뉴스 역시 마찬가지 방식으로 유저에게 보인다. <del>한국은 정치에선 미국보다 더 선진국?</del> )

지난 번 [필터 버블](http://flyhendrixfly.net/%eb%8b%b9%ec%8b%a0%ec%9d%98-%ed%95%84%ed%84%b0-%eb%b2%84%eb%b8%94%ec%9d%b4-%eb%af%bc%ec%a3%bc%ec%a3%bc%ec%9d%98%eb%a5%bc-%ed%8c%8c%ea%b4%b4%ed%95%9c%eb%8b%a4wired-nov-7-2016/) 포스팅은 그런 메시지 증폭 상황에서 어떻게 민주당 리버럴들이 꼼짝없이 당했는지에 대해서 다룬다면, 이번 글은 트럼프가 어떻게 이겼는지에 포커스를 맞춘다. **<a href="http://flyhendrixfly.net/%ec%83%88%eb%a1%9c%ec%9a%b4-%eb%b0%a9%ec%8b%9d%ec%9d%98-%ec%a1%b0%ec%a7%81%ed%99%94/" target="_blank">오바마의 2012년 재선으로 &#8216;빅 데이터&#8217;를 활용한 맞춤형 선거운동은 &#8216;필승 전략&#8217;으로 민주당에서 여겨졌다</a>.** 기존의 선거전문가 대신 통계전문가와 실리콘 밸리 출신 데이터 과학자들을 고용했다.[네이트 실버](http://fivethirtyeight.com)가 스타가 됐고, 여론조사는 확장되어 베이즈 통계를 활용한 실시간 예측분석으로 구사됐다. 실시간으로 확률이 엎치락 뒤치락 하는 &#8216;게임&#8217;을 사람들은 목격했다. &#8216;숫자&#8217;로 말하면 &#8216;신호&#8217;를 잡아내 이길 거라는 확신이 있었다. 힐러리 클린턴은 2012년보다 훨씬 더 예산을 증액해 데이터-기반 선거를 진행했다.

**사실 선거를 &#8216;게임&#8217;으로 느낄 수 있었던 것은, 멍청한 공화당이 스마트한 민주당을 이길리 없다는 미국 리버럴의 자기 오만도 있었다**. 그러나 선거 패배 이후 미국 리버럴들의 &#8216;멘붕&#8217;은 끊이지 않는 것 같다. 정신승리와 &#8216;국개론&#8217;까지 한국에서도 많이 목격했던 행태다. 어쨌든 미국 리버럴의 테크 맹신과 정세 분석에 대한 편향에 대해서는 기회가 날 때 다시 쓸 수 있을 것이다.

&nbsp;

<img class="alignnone size-full" src="http://cdn.static-economist.com/sites/default/files/imagecache/full-width/images/2016/11/articles/main/20161119_usp509.jpg" alt="" width="595" height="335" />

<a href="http://www.economist.com/news/united-states/21710614-fake-news-big-data-post-mortem-under-way-role-technology" target="_blank">원문: The Role of Technology in the Presidential Election</a>

_**짝퉁 뉴스부터 빅데이터까지, 사후진단이 한참**_

<span style="font-weight: 400;">미국의 대통령 선거 초반부, 전문가들은 힐러리 클린턴과 도널드 트럼프의 대결을, 거대한 유조선과 소말리아 해적의 싸움과 비교했다. 이는 디지털 캠페인에 있어 부분적으로 사실임이 드러났다. 거대한 데이터 전함은 혼돈의 소셜 미디어 소함대에게 패배했다. 지금 중요한 질문은 이 현상이, 미국과 다른 나라의 미래 선거에 무엇을 의미하는지다.</span>

<span style="font-weight: 400;">클린턴의 선거는 단언컨데 미국 역사상 가장 데이터-주도적이었다. 그녀의 조직은 예컨대 친절한 자원봉사자들이 방문해 시민의 의무를 상기시키는 게 도움이 되는 게 어떤 유권자인지를 결정하는 통계적 모델까지 설계했던 수십명의 데이터 과학자를 고용했다. 선거 캠페인의 마스터 프로그램은 2012년 오바마의 재선을 도왔던 프로그램보다 하루에 6배 많은 시뮬레이션을 실행해냈다.</span>

<span style="font-weight: 400;">그런 요인들이 자만심을 자라게 했을 수 있다. 그녀의 캠페인은 “데이터가 전하는 것에 대한 지나친 믿음을 가지고 있었을 수도 있다”고 노스 캐롤라이나 대의 선거 캠페인과 데이터 전문가인 Daniel Kreiss가 전한다. 1992년 이래 민주당 대선후보를 찍어왔던 미시간에서는, 클린턴은 무방비 상태로 당했다. 트럼프는 여론조사에서 한참 뒤지는 결과를 받았음에도, 미시간을 빈번하게 방문했다. 선거 막판 미시간 주의 취약함이 드러나고, 오바마 대통령이 더 이상의 출혈을 막기 위해 부랴부랴 지원유세를 나갔지만 이미 때는 늦었다.</span>

<span style="font-weight: 400;">모든 통계 모델은 일련의 가정을 전제한다. 가정이 성립되지 않으면, 결과 예측은 “편향”될 수 있고, 통계학자는 잘못된 것을 말할 수 있다. 좀 더 직설적인 선수들은 그걸 다른 말로 표현한다. “쓰레기를 넣으면, 쓰레기가 나온다.”(Garbage in, garbage out.) 예비 선거에서 클린턴에게 패한, 버니 샌더스의 고위 고문이었던 2명은 그녀의 캠페인이 부주의하게 그녀의 라이벌(트럼프)에게 투표할 가능성이 있는 부동층 유권자(swing voters)들을 부추켰을 수 있다고 주장했다.</span>

<span style="font-weight: 400;">반면, 트럼프는 데이터를 “과대 평가된 것으로&#8221; 여겨 묵살했다. 트럼프 캠프는 오직 6월에 런던에 있는 회사인 Cambridge Analytica를 고용했을 뿐이다. 7월에 트럼프가 공화당 대선후보 지명을 받고나서, 그는 공화당의 디지털 시스템을 사용할 수 있었지만, 그것들은 민주당에 비하면 덜 정교한 것으로 치부됐다.</span>

<span style="font-weight: 400;">트럼프의 데이터 팀은 승리로 가는 길을 찾는 데 도움을 준 것으로 보인다. 조기 투표와 부재자 투표가 농촌 유권자의 증가를 보여줬다고 Cambridge Analytica의 Matt Oszkowski는 설명한다. 트럼프 캠프는 농촌 유권자들을 더 참여시키는 노력을 배가했다. 그들은 농촌 투표 독려가 전통적인 민주당 성향의 주에서 여론조사 격차를 줄일 수 있으리라고 배팅했고, 실제 결과로도 드러났다.</span>

<span style="font-weight: 400;">하지만 트럼프 승리에 어떤 테크놀로지가 기여했다면, 그건 데이터 과학이라기보다는 소셜 미디어일 것이다. 트럼프와 그의 캠페인 수석이었고, 현재는 수석 전략가인 Steve Bannon은 페이스북과 트위터가 이끄는 미디어 환경이 선거에 어떻게 작용하는지를 이해했다. 뉴스 한 편이 온라인으로 퍼져 나가는 것은 그 진실성과 일관성 때문이 아니라, 그 뉴스가 놀랍고 충격적이며 편견을 확인해 주는지 여부에 달렸다는 것이다. 심지어 그 뉴스 내용이 명백히 거짓이라도, 가상의 에코 챔버(echo chamber: 반향실) 안에서는 끊임 없이 튀어 다닐 수 있는 것이다.</span>

<span style="font-weight: 400;">이 현상은 부분적으로 페이스북에서 두드러졌다. 페이스북 알고리즘은 사이트 내부에서 댓글을 달거나 공유하게 해 유저를 최대한 붙잡아 두기 위해 이미 보여줬던 최적화된 콘텐츠 유형을 유저에게 제공하는 방식의,  “참여&#8221;를 최대로 만들기 위해 조정된다. “트럼프와 그의 캠프는 본질적으로 페이스북의 알고리즘을 해킹한 거죠.” 조지 워싱턴 대학의 Matthew Hindman은 전한다. 수많은 온라인 간행물은 친-트럼프 선전물과, 꾸준한 흐름의 짝퉁 뉴스를 쏟아냈다. 좌파 사이트들도 그런 방식으로 수많은 내용을 전했지만, 그들의 화력은 트럼프 캠프에 비하면 양적으로 적었던 것으로 보인다. 트럼프의 가장 값진 미디어는 현재 1천5백4십만여 명이 팔로우 하는 트위터 피드였다. 주류 미디어가 종종 충격적인 그의 트위터를 끄집어 보도할 때, 이는 트럼프를 주목하게 만들고 수십억 달러 공짜 광고를 그에게 전달했다. (표 참조)<img class="alignleft" src="http://cdn.static-economist.com/sites/default/files/imagecache/original-size/images/2016/11/articles/body/20161119_woc509_0.png" alt="" width="388" height="412" /></span>

<span style="font-weight: 400;">이게 선거에 있어 얼마나 영향을 미쳤는지는 이미 토론의 주제다. 몇몇은 클린턴의 패배가 데이터와 통계 방법에 너무 의존하는 것의 위험을 증명한다고 주장한다. “우리는 몇몇 과학을 버리고, 기예(art)에 좀 더 집중할 필요가 있어요.” 좌파 선거 집단인 혁명 메시징(Revolution Messaging)을 운영하고, 버니 샌더스 선거 운동의 디지털 분야를 맡았던, Scott Goodstein이 전한다. 선거운동은 기술(technology)에 많이 의존했지만, 종종 인간의 손길로 만든 것이기도 했다. 자원봉사자들이 개인적으로 문자메시지를 보내 재빠르게 집회를 조직할 수 있게 해준 메신저 앱인 ‘허슬Hustle’ 앱은 중요한 도구였다.</span>

<span style="font-weight: 400;">소셜 미디어의 역할은 더 많은 관심을 모아내는 데 있다. 페이스북으로 하여금 짝퉁 뉴스를 필터할 수 있게 알고리즘을 변경하라는 압력이 가중되고 있다. 처음에 페이스북은 그 사실을 부인했다. 페이스북의 대표인 마크 주커버그는 선거 후에 열린 한 회의에서, 짝퉁</span>

 <span style="font-weight: 400;">뉴스가 선거에 영향을 미쳤다는 생각을 “완전히 정신 나간 것&#8221;으로 간주했다. 하지만 이런 입장은 딴세상에서나 가능해 보인다. 거의 절반에 달하는 미국 성인들이 이제 정치뉴스를 페이스북에서 찾아 읽는다.</span>

<span style="font-weight: 400;">페이스북은 그 이후로 다소나마 입장을 바꿨다. 다른 온라인 거물인 구글은 11월 14일자로 짝퉁 뉴스가 구글의 광고 서비스를 이용하는 것을 차단하겠다고 발표했고, 페이스북은 재빠르게 같은 짝패를 냈다. (하루가 지나자 트위터는 미국의 새로운 극우파 운동으로 불리는 “alt-right” 유명인(personalities)들의 계정을 정지시켰다.) 11월 19일 주커버그는 좀 더 구체적인 블로그 포스팅을 통해, 소셜 미디어가 그 문제를 어떻게 처리할 수 있는지를 설명했다. 사람들이 가짜 스토리를 신고하기 쉽게 만들고, 쓸만한 팩트-체크 조직에 확인할 수 있는 등의 조치가 대책으로 마련됐다. 하지만 주커버그는 페이스북 자체는 어떤 내용이 가짜인지 아닌지를 결정하길 원하지 않는다고 강조했다. 주커버그는 “우리는 페이스북 스스로 진리를 중재하고 싶지 않고, 그 역할은 우리들의 공동체와 신뢰할 수 있는 제3자에게 맡기려 한다”고 썼다.</span>

<span style="font-weight: 400;">트럼프가 소셜 미디어에서 성공한 것은 트럼프의 성격과 공격에 특별히 취약했던 라이벌(힐러리)의 특성이라는, 일련의 독특한 환경의 결과일 수 있다. 하지만 영국의 브렉시트 국민투표 때도 역시나 소셜 미디어는 반쪽짜리 진실과 명백한 거짓말을 전파하는 데 중요한 역할을 했다. 극우파 국민전선의 마리 르 펜 후보가 본선에 올라갈 것으로 예상되는 4월의 프랑스 대선은, 거대한 온라인 플랫폼이 얼마나 큰 영향을 미칠 수 있는 지 확인할 수 있는 시범 사례가 될 것이다. 페이스북이나 트위터 같은 거대한 온라인 플랫폼 회사들은 자신들이 테크 회사라며 논쟁 뒤에 오랫동안 숨어 있었다. 트럼프의 승리 이후 이러한 포지션은 결코 설득력도 없고, 훨씬 더 공허한 벨소리로 울릴 따름이다.</span>

(The Economist, Nov, 20, 2016)
