.card {
  width: 250px;
  background: rgb(44, 44, 44);
  font-family: 'Courier New', Courier, monospace;
  border-top-left-radius: 12px;
  border-top-right-radius: 12px;
  border-bottom-left-radius: 4px;
  border-bottom-right-radius: 4px;
  overflow: hidden;
}

.card__title {
  color: white;
  font-weight: bold;
  padding: 5px 10px;
  border-bottom: 1px solid rgb(167, 159, 159);
  font-size: 0.95rem;
}

.card__data {
  font-size: 0.8rem;
  display: flex;
  justify-content: space-between;
  border-right: 1px solid rgb(203, 203, 203);
  border-left: 1px solid rgb(203, 203, 203);
  border-bottom: 1px solid rgb(203, 203, 203);
}

.card__right {
  width: 60%;
  border-right: 1px solid rgb(203, 203, 203);
}

.card__left {
  width: 40%;
  text-align: end;
}

.item {
  padding: 3px 0;
  background-color: white;
}

.card__right .item {
  padding-left: 0.8em;
}

.card__left .item {
  padding-right: 0.8em;
}

.item:nth-child(even) {
  background: rgb(234, 235, 234);
}
