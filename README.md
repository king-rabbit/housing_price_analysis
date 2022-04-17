# 보금자리론 주택 가격 기준 분석

미디어 플랫폼인 쏘프라이즈(현 얼룩소) 질문에 대한 답변(https://alook.so/posts/QE7tOP)으로 제출한 내용입니다.


data
- apartment_purchase_data: 아파트 매매 실거래가 데이터
    - 2016년부터 2021년 5월까지의 데이터이며, 2020년 데이터는 양이 많아 2개로 나뉘어져 있습니다.
    - 아파트매매_2008_2009.csv: 2008년 5월 ~ 2010년 4월까지 서울시 아파트 매매 데이터만 담고 있습니다.
    - 실거래가 데이터 리포지토리(https://github.com/vuski/RealEstateTransactionKorea) 및 국토교통부 실거래가 공개시스템(http://rtdown.molit.go.kr/) 데이터를 취합했습니다.
    
- geo_data: 17개 광역시도별 행정구역 및 시군구별 행정구역 geojson 파일입니다.
    - 'GIS DEVELOPER'에서 제공한 대한민국 최신 행정구역 SHP 파일(http://www.gisdeveloper.co.kr/?p=2332)을 geojson으로 변환했습니다.

- mortgage_data: 주택금융시스템(https://www.hf.go.kr/hf/index.do)에서 제공하는 보금자리론 대출실적 데이터
 
    
graphs: 시각화된 각종 그래프를 html로 저장

analysis.ipynb: 분석 주피터노트북 파일
- pyecharts 등 라이브러리 설치가 요구되며, mapbox token을 발급받으셔서 token 변수에 넣으시면 지도 시각화를 할 수 있습니다.
- pyecharts 라이브러리 문제로 jupyter lab보다는 jupyter notebook으로 보시는 걸 추천합니다.
