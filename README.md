# pro06 springboot

```
## 테이블
1. member - 쇼핑몰 회원 정보 테이블
2. cart - 회원의 장바구니 목록 테이블
3. cart_item - 장바구니에 담긴 상품 정보 테이블
4. orders - 쇼핑몰 회원들의 주문 목록 테이블
5. order_item - 주문된 상품 정보 테이블
6. product - 쇼핑몰 상품 정보 테이블
7. item_img - 상품에 대한 이미지 정보를 담고 있는 테이블
```

```
create table product(
	proNo int primary key auto_increment, -- 제품 번호
	cateNo int not null, -- 카테고리 1번 top 2번 bottom 3번 shoes
	proName varchar(40) not null, -- 상품 이름
	proSpec varchar(500), -- 상품 설명
	oriPrice int not null, -- 원가
	discountRate double not null, -- 할인율
	proPic varchar(200), -- 사진
	proPic2 varchar(200), -- 사진
    scnt int default 0, -- 조회수?
    regdate datetime default now(), -- 등록일자
    amount int default 0 -- 재고수량
);
```
