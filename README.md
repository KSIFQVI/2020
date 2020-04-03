It's 2020 KSIF QVI's First project

<< Portfolio() 변수명 정의 >>
Variable name	Description	Dtype	Unit	Example	비고
code	코드	object		A000020	
code02	코드	object		A000020_0	
firmname	회사이름	object			
mdate	Trading Day	object			
date	Day	datetime64[ns]			
size	로그 시가총액	float64			
e_p	1 / PER	float64			Infinite 존재
b_p	1 / PBR	float64			
s_p	1 / PSR	float64			
gp_p	1 / PGPR (주가매출 총이익비율)	float64			
op_p	1 / POPR	float64			
c_p	1 / PCR	float64			
roa	ROA	float64			
roe	ROE	float64			
roic	ROIC	float64			
gp_a	GP / Asset	float64			
gp_s	GP / Sales	float64			
salesqoq	분기별 Sales 증가율	float64			
gpqoq	분기별 GP 증가율	float64			
roaqoq	분기별 ROA 증가율	float64			
prior_2_6	모멘텀, 6달전부터 2달전까지	float64			https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/Data_Library/det_mom_factor.html
prior_2_12	Fama French Factor, 12개월~2개월전까지 모멘텀	float64			https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/Data_Library/det_mom_factor.html
liq_ratio	Current Asset / Current Liability	float64			
equity_ratio	Equity / Total Asset	float64			
debt_ratio	Liability / Total Asset	float64			
foreign_ownership_ratio	외국인 보유비율	float64			
ret	Return	float64			
prcoadj_hypo	Open(시초가)	float64			
prchadj_hypo	High	float64			
prcladj_hypo	Low	float64			
prccadj_hypo	Close(종가)	float64			
vol_won	거래대금 (거래량 X 주식가격)	float64			
me	시가총액(Market Equity)	float64			
atq	총자산(Total Assest)	float64	1000원단위		
ltq	총부채(Total Liabilities)	float64	1000원단위		
seqq	총자본(Total Equity)	float64	1000원단위		
retained_earnings	Retained Earnings	float64	1000원단위		
revtq	총매출(Total Revenue) - 1분기	float64	1000원단위		
revtq4	총매출(Total Revenue) - 직전 4분기 합	float64	1000원단위		
niq	당기순이익(Net Income from continuing Operations) - 1분기	float64	1000원단위		
niq4	당기순이익(Net Income from continuing Operations) - 직전 4분기 합	float64	1000원단위		
opq	영업이익(Operating Profit) - 1분기	float64	1000원단위		
opq4	영업이익(Operating Profit) - 직전 4분기 합	float64	1000원단위		
actq	유동자산(Current Assets)	float64	1000원단위		
lctq	유동부채(Current Liability)	float64	1000원단위		
wc	Working Capital	float64	1000원단위		
per	PER	float64	1000원단위		
pbr	PBR	float64	1000원단위		
exchcd	거래소 (KSE, KOSDAQ)	object			
trading_halt	거래정지(거래정지 일수)	float64			
traded	총거래일수  - 거래정지	float64			
trading_halt_during_month	해당 달에서 거래정지 여부(0: 거래정지 안된거, 1:거래정지 된거)	int64			
managed	관리종목(관리종목 된 일수)	float64			
managed_during_month	해당 달에서 관리종목 여부(0: 관리종목 된거, 1: 관리종목 안된거)	int64			
listed_month_begin	월초에 상장 되어있는 여부(1이 상장 되어있는거) - 1밖에 없음	int64			
delisted	해당 달에서 상폐된 종목(0: 상폐 안된거, 1: 상폐된거)	int64			
numobs	거래일수(trading_halt + traded)	int64			
trading_halt_during_month_LEAD_1	다음 달에서 거래정지 여부(0: 거래정지 안된거, 1:거래정지 된거)	float64			
managed_during_month_LEAD_1	다음 달에서 관리종목 여부(0: 관리종목 된거, 1: 관리종목 안된거)	float64			
delisted_LEAD_1	해당 달에서 상폐된 종목(0: 상폐 안된거, 1: 상폐된거)	float64			
trading_halt_reason	거래정지 선정 사유	object			
managed_reason	관리종목 선정 사유	object			
investment_treatment	투자 주의 및 경고	object			투자주의 별이 있는거 없는거 있음
fn_sector_code	FN 가이드 섹터 코드	object		FGSC.30	
fn_sector	섹터 설명	object		필수소비재	
fn_industry_group_code	FN 가이드 산업군 코드	object		FGSC.30.20	
fn_industry_group	산업군 설명	object		음식료 및 담배	
fn_industry_code	FN 가이드 산업 코드	object		FGSC.30.20.20	
fn_industry	산업 설명	object		식료품	
kospi100	KOSPI 200 중에서 시총 기준 상위 100개	object		Y / N	
kospi200	KOSPI 200	object		Y / N	
audit_opinion	감사의견	object		적정의견	
ret_1m	수익률(최근 1개월)	float64			빨간것들은 단위가 .. Machine learning 돌리려고, 우리가 흔히 아는 단위가 아닐수 있으니 체크
ret_2m	수익률(최근 2개월)	float64			예를들면, 샤프는 (1+ret)/(1+vol)
ret_3m	수익률(최근 3개월)	float64			
ret_4m	수익률(최근 4개월)	float64			
ret_5m	수익률(최근 5개월)	float64			
ret_6m	수익률(최근 6개월)	float64			
vol_1m	거래량(최근 1개월)	float64			
vol_2m	거래량(최근 2개월)	float64			
vol_3m	거래량(최근 3개월)	float64			
vol_4m	거래량(최근 4개월)	float64			
vol_5m	거래량(최근 5개월)	float64			
vol_6m	거래량(최근 6개월)	float64			
sharpe_1m	sharpe ratio(최근 1개월)	float64			
sharpe_2m	sharpe ratio(최근 2개월)	float64			
sharpe_3m	sharpe ratio(최근 3개월)	float64			
sharpe_4m	sharpe ratio(최근 4개월)	float64			
sharpe_5m	sharpe ratio(최근 5개월)	float64			
sharpe_6m	sharpe ratio(최근 6개월)	float64			
ret_1m_LEAD_1	수익률(1달 후)	float64			
ret_2m_LEAD_2	수익률(1달 후부터 2달 후까지)	float64			
ret_3m_LEAD_3	수익률(1달 후부터 3달 후까지)	float64			
ret_4m_LEAD_4	수익률(1달 후부터 4달 후까지)	float64			
ret_5m_LEAD_5	수익률(1달 후부터 5달 후까지)	float64			
ret_6m_LEAD_6	수익률(1달 후부터 6달 후까지)	float64			
vol_1m_LEAD_1	거래량(1달 후)	float64			
vol_2m_LEAD_2	거래량(1달 후부터 2달 후까지)	float64			
vol_3m_LEAD_3	거래량(1달 후부터 3달 후까지)	float64			
vol_4m_LEAD_4	거래량(1달 후부터 4달 후까지)	float64			
vol_5m_LEAD_5	거래량(1달 후부터 5달 후까지)	float64			
vol_6m_LEAD_6	거래량(1달 후부터 6달 후까지)	float64			
sharpe_1m_LEAD_1	sharpe ratio(1달 후)	float64			
sharpe_2m_LEAD_2	sharpe ratio(1달 후부터 2달 후까지)	float64			
sharpe_3m_LEAD_3	sharpe ratio(1달 후부터 3달 후까지)	float64			
sharpe_4m_LEAD_4	sharpe ratio(1달 후부터 4달 후까지)	float64			
sharpe_5m_LEAD_5	sharpe ratio(1달 후부터 5달 후까지)	float64			
sharpe_6m_LEAD_6	sharpe ratio(1달 후부터 6달 후까지)	float64			
vol_won_me	거래량/시총	float64			
vol_won_me_12	거래량/시총 12개월 평균	float64			
vol_won_12	거래량 12개월 평균	float64			
me_12	시총 12개월 평균	float64			
mov5y_trading_halt	지난 5년 거래정지 일수	float64			
mov3m_trading_halt	지난 3개월 거래정지 일수	float64			
mov3m_managed	지난 3개월 관리종목지정 일수	float64			
vol_won_me_12_rank	거래량/시총 12개월 cross sectional 순위	float64			
me_12_rank	시총 12개월 평균 cross sectional 순위	float64			
fin_score	트러스톤 financial stability score	float64			
fin_score_rank	트러스톤 financial stability score의 cross-sectional 순위	float64			
fin_score_12	트러스톤 financial stability score의 12개월 평균	float64			
fin_score_12_rank	트러스톤 financial stability score의 12개월 평균의 cross-sectional 순위	float64			
fin_score_24	24개월	float64			
fin_score_24_rank	24개월 순위	float64			
truston_universe	xmfj	int64			
whole_universe	더미 변수, 1, 0, 트러스톤 유니버스에 들어가면 1	int64			
qvi_universe	더미 변수, 1, 0, QVI 유니버스에 들어가면 1, 좀더 스몰스탁위주	int64			
lag1_me	시가총액의 1개월 래그	float64			
vol_won_12_rank	거래량 12개월 평균의 cross-sectional 평균	float64			
prco	Open(시초가)	float64			
prch	High	float64			
prcl	Low	float64			
prcc	Close(종가)	float64			
vwret_korea	한국시장 전체 시총 가중 평균 리턴(KOSPI랑 KOSDAQ)	float64			
vwret_kospi	코스피 시총 가중 평균 리턴	float64			
vwret_kospi200	코스피 200 시총가중평균 리턴	float64			
vwret_kosdaq	코스닥 200 시총가중평균 리턴	float64			
