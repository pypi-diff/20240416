# Comparing `tmp/FreeBack-3.0.0b0.tar.gz` & `tmp/FreeBack-3.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-3.0.0b0.tar", last modified: Fri Apr 12 01:46:35 2024, max compression
+gzip compressed data, was "FreeBack-3.0.1a0.tar", last modified: Tue Apr 16 09:36:06 2024, max compression
```

## Comparing `FreeBack-3.0.0b0.tar` & `FreeBack-3.0.1a0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.628241 FreeBack-3.0.0b0/
-drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.621129 FreeBack-3.0.0b0/FreeBack/
--rw-rw-rw-   0        0        0       77 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/__init__.py
--rw-rw-rw-   0        0        0    39318 2024-04-09 06:54:26.000000 FreeBack-3.0.0b0/FreeBack/alpha.py
--rw-rw-rw-   0        0        0    33890 2024-04-11 00:53:14.000000 FreeBack-3.0.0b0/FreeBack/barbybar.py
--rw-rw-rw-   0        0        0    12401 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/display.py
--rw-rw-rw-   0        0        0    10145 2024-03-01 16:35:30.000000 FreeBack-3.0.0b0/FreeBack/event.py
--rw-rw-rw-   0        0        0    15629 2024-04-10 06:43:08.000000 FreeBack-3.0.0b0/FreeBack/my_pd.py
--rw-rw-rw-   0        0        0    35542 2024-04-11 06:17:47.000000 FreeBack-3.0.0b0/FreeBack/post.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:46:35.627232 FreeBack-3.0.0b0/FreeBack.egg-info/
--rw-rw-rw-   0        0        0     1182 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 01:46:35.000000 FreeBack-3.0.0b0/FreeBack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2024-04-12 01:34:50.000000 FreeBack-3.0.0b0/LICENSE
--rw-rw-rw-   0        0        0     1182 2024-04-12 01:46:35.627232 FreeBack-3.0.0b0/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-04-11 06:54:48.000000 FreeBack-3.0.0b0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 01:46:35.628241 FreeBack-3.0.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-12 01:43:09.000000 FreeBack-3.0.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.862022 FreeBack-3.0.1a0/
+drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.829229 FreeBack-3.0.1a0/FreeBack/
+-rw-rw-rw-   0        0        0       77 2024-04-11 06:17:47.000000 FreeBack-3.0.1a0/FreeBack/__init__.py
+-rw-rw-rw-   0        0        0    40491 2024-04-16 09:31:17.000000 FreeBack-3.0.1a0/FreeBack/alpha.py
+-rw-rw-rw-   0        0        0    33890 2024-04-11 00:53:14.000000 FreeBack-3.0.1a0/FreeBack/barbybar.py
+-rw-rw-rw-   0        0        0    12401 2024-04-11 06:17:47.000000 FreeBack-3.0.1a0/FreeBack/display.py
+-rw-rw-rw-   0        0        0    10140 2024-04-12 10:51:57.000000 FreeBack-3.0.1a0/FreeBack/event.py
+-rw-rw-rw-   0        0        0    15629 2024-04-10 06:43:08.000000 FreeBack-3.0.1a0/FreeBack/my_pd.py
+-rw-rw-rw-   0        0        0    35554 2024-04-16 07:31:49.000000 FreeBack-3.0.1a0/FreeBack/post.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:36:06.861025 FreeBack-3.0.1a0/FreeBack.egg-info/
+-rw-rw-rw-   0        0        0     1232 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 09:36:06.000000 FreeBack-3.0.1a0/FreeBack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2024-04-12 01:34:50.000000 FreeBack-3.0.1a0/LICENSE
+-rw-rw-rw-   0        0        0     1232 2024-04-16 09:36:06.861025 FreeBack-3.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2024-04-15 01:34:55.000000 FreeBack-3.0.1a0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:36:06.862022 FreeBack-3.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-04-16 07:24:51.000000 FreeBack-3.0.1a0/setup.py
```

### Comparing `FreeBack-3.0.0b0/FreeBack/alpha.py` & `FreeBack-3.0.1a0/FreeBack/alpha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pandas as pd
 import numpy as np
 from scipy import stats
 import statsmodels.api as sm
 from FreeBack.post import matplot
-#from FreeBack.my_pd import parallel
 from FreeBack import my_pd
-import datetime, copy
-
+import os
 # 该模块包含：
 # 因子计算常用函数
 # 单因子与多因子检验模块（组合法、回归法）
 
 
 #######################################################################################################
 ####################################### 因子计算常用函数 #################################################
@@ -65,15 +63,15 @@
     df['yesterday_th'] = df['th'].groupby('code').shift()
     df = df.fillna(getattr(df.index[0][0], freq))
     df['after'] = df.apply(lambda x: x[0] if x.th!=x.yesterday_th else np.nan, axis=1)
     df = df.groupby('code').fillna(method='ffill')
     df = df.groupby('code').fillna(method='bfill')
     return df['after']
 # 直接只选用原数据的周初、月初值
-# 没有周一和1号的月份用下一个第一个出现的值
+# 没有周一和1号的月份用下一个第一个出现的值***
 def resample_select(market, freq='month'):
     if freq=='month':
         return market[market.index.map(lambda x:getattr(x[0], 'day'))==1]
     elif freq=='week':
         return market[market.index.map(lambda x:getattr(x[0], 'weekday')())==0]
 def QQ(factor, date=None):
     plt, fig, ax = matplot(w=6, d=4)
@@ -98,98 +96,230 @@
     # factorgroup
 # 2. 回归法， 假设截面上因子与未来收益率线性相关，计算该线性关系的一系列统计量。
     # Reg
 
 ########################################## 组合法 #######################################################
 
 class Portfolio():
-# factor pd.Series, multiindex(date,code)    T日因子值,数据类型为float 
-# price T日交易价格(使用后一天开盘价或者VWAP等是接近实际情况的，用来确定权重、收益率) 
-# divide 输入模式1，tuple,给出全部阈值确定连续分组； 输入模式2， list， 给出每个分组的前后阈值。
-# periods 轮动的时间间隔
-# returns 默认情况下使用T-1日到T日price计算收益率,也可以直接接收定义，格式为index is date  columns is code， value is 收益率 空值补0
-# holdweight T日的投资组合权重，默认等权
-# comm 每次换手的交易成本，默认为0
-# norm 是否将因子值截面转化为排序值（0到1），默认开启 
+# factor 数据类型pd.Series, multiindex(date,code)   T日因子值(可以在此排除涨停板)
+# price 数据类型pd.Series, multiindex(date,code) T日交易价格(最宽松情况可以使用当日收盘价，\
+# 使用后一天开盘价或者VWAP等是接近实际情况的(全市场数据即可) 
+# norm 是否按照因子值的排序来对投资组合分组,默认开启。否则使用原始因子值进行分组 
+# divide 
+# 数据类型为tuple时，给出全部阈值确定连续分组；
+# 数据类型为list， 给出每个分组的前后阈值,例：[(0,0.1),(0.9,1)]表示选取最小10%和最大10%构建组合，前开后闭。
+# norm开启时，元素<=1时表示百分比，大于1时表示绝对数量，如(0,0.2)表示持有钱20%，(0，10)表示持有前十只。
+# 否则表示因子值的阈值。
 # justdivide 是否仅计算给出分组的收益而不计算全市场组合收益，默认计算全市场组合收益(权重由holdweight确定)
-# 当日收益率为当日收盘价相对昨日收盘价收益率*前一日持仓权重
-# 作弊模式    当日因子确定当日持仓 
-# holdweight 持仓权重矩阵  例如流通市值
-# comm 不影响结果，仅仅在result中给出多头费后年化收益率 
-    def __init__(self, factor, price, divide=(0, 0.2, 0.4, 0.6, 0.8, 1), periods=(1, 5, 20), \
-                 returns=None, holdweight=None, comm=0, norm=True, justdivide=False):
+# periods (1, 5, 20)同时计算1天5天20天轮动的结果
+# holdweight pd.Series, multiindex(data,code)  T日的投资组合权重，默认等权
+# comm 每次单边换手的交易成本，默认为0
+## 当日收益率为当日收盘价相对昨日收盘价收益率*前一日持仓权重
+## comm 不影响结果，仅仅在result中给出多头费后年化收益率 
+    def __init__(self, factor, price, norm=True, divide=(0, 0.2, 0.4, 0.6, 0.8, 1),\
+                 justdivide=False, periods=(1, ), \
+                  holdweight=None, comm=0):
         self.comm = comm
         self.norm = norm
         self.justdivide=justdivide
+        # 一个确定持有张数（不去除停牌），一个确定收益率(去除停牌)
+        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
+        # 每日收益率(当日收盘相比上日收盘)
+        returns = self.price/self.price.shift() - 1
+        self.returns = returns.fillna(0)
 #        # 先按照截面排序归一化
         if norm:
             self.factor = Rank(pd.DataFrame(factor.rename('factor')))
         else:
             self.factor = pd.DataFrame(factor.rename('factor'))
         self.variable = factor
-        # 一个确定持有张数（不去除停牌），一个确定收益率(去除停牌)
-        self.price = pd.DataFrame(price.rename('price')).pivot_table('price', 'date' ,'code')
-        # 每日收益率(当日收盘相比上日收盘)
-        if type(returns) == type(None):
-            returns = self.price/self.price.shift() - 1
-            returns = returns.fillna(0)
-            self.returns = returns
-        else:
-            self.returns = returns
         # 组合权重 
         if type(holdweight) != type(None):
-            # 退市后即为0
+            # 没有权重则按0计
             holdweight = holdweight.fillna(0)
             self.holdweight = holdweight.apply(lambda x: x/x.sum(), axis=1)
         else:
             self.holdweight = None
         # 结果dataframe 行：时间周期  列：IC、ICIR（分组计算的IC、ICIR(非rank)）、 多空组合收益、多头收益、 等权收益、
         # 考虑换手率多空收益、 夏普、 多空平均换手率
         self.result = pd.DataFrame(columns=['group IC', 'group ICIR', 'L&S return', 'L return',\
                  'market return', 'L&S sharpe', 'L sharpe', 'market sharpe', 'real return', \
                     'real sharpe', 'turnover'])
         self.result.index.name = 'holding period'
         # 运行
         self.run(divide, periods)
     def run(self, divide, periods):
+        self.divide = divide
         self.periods = periods
-        # 如果是list则直接为a_b
-        if type(divide) == type(list()):
-            # 代理变量绝对值
-            if self.norm == True:
-                self.threshold = [self.variable.groupby('date').quantile(divide[0][0])] +\
-                  [self.variable.groupby('date').quantile(i[1]) for i in divide]
-            else:
-                self.threshold = [ i for i in divide]
-            self.a_b = divide
-        # 选取factor区间[(0,0.2),(0.2,0.4)...]
+        # self.a_b表示对因子分隔的阈值，如果是list则直接为a_b
+        if type(self.divide) == type(list()):
+            self.a_b = self.divide
+        # 如果是tuple则转化成list
         else:
-            if self.norm==True:
-                self.threshold = [self.variable.groupby('date').quantile(i) for i in divide]
-            else:
-                self.threshold = [i for i in divide]
-            self.a_b = [(divide[i],divide[i+1]) for i in range(len(divide)-1)]
-        # 如果justdivide = True不计算(0，1)
+            self.a_b = [(self.divide[i],self.divide[i+1]) for i in range(len(self.divide)-1)]
+        # 如果justdivide为False,则增加一个可以选中全部标的的组合
         if not self.justdivide:
             if self.norm == True:
-                self.a_b = self.a_b + [(0,1)]
+                # 按百分比划分
+                if self.a_b[-1][1]<=1:
+                    self.a_b = self.a_b + [(0,1)]
+                else:
+                    self.a_b = self.a_b + [(0, 99999)]
             else:
                 self.a_b = self.a_b + [(self.factor.min().values[0], self.factor.max().values[0])]
     # 生成持仓表 -> 获得 df_contri(index date  columns code) -> 获得净值每日对数收益率 -> 获得换手率
     # 全部为矩阵操作
         self.matrix_hold()
         self.matrix_contri()
         self.matrix_lr()
         self.matrix_holdn()
         self.matrix_turnover()
         if not self.justdivide:
             self.get_result()
+# mat[period][factor range]  list[factor range]
+# 获得每个持仓周期 每个因子区间的虚拟持仓(只保证比例关系正确) 
+# a_b factor range from a to b 区间内市值等权重
+    def matrix_hold(self):
+    # 每个bar按标的等权配置需要的持仓
+        if self.norm:
+            if self.a_b[-1][1]<=1:
+                look_factor = self.factor.groupby('date').rank(pct=True)
+            else:
+                print('整数排序')
+                look_factor = self.factor.groupby('date').rank()
+        else:
+            look_factor = self.factor
+        look_factor = look_factor.reset_index()
+        # 选取因子值 满足a_b list中全部条件的 放置于list_hold (前开后闭，与Rank函数返回的(0，1]对应)
+        bar_hold = [look_factor[(i[0]<look_factor['factor']) &\
+                                 (look_factor['factor']<=i[1])] for i in self.a_b]
+        # 每一组合选中的标的个数
+        self.group_number = [i.groupby('date').count() for i in bar_hold]
+        # 在date没有出现的code补np.nan
+        bar_hold = [pd.DataFrame(i.pivot_table('factor', 'date', 'code'),\
+                                 index=self.factor.index.get_level_values(0).unique())\
+                                     for i in bar_hold]
+        # 等权情况下持有标的的持仓数量为 1/price（持仓金额相等）
+        #bar_hold = [(i.isnull().replace([True,False],[0,1])*\
+        #             (1/self.price)).fillna(0) for i in bar_hold]
+        bar_hold = [((~i.isnull()).astype(int)*\
+                     (1/self.price)).fillna(0) for i in bar_hold]
+        # 当holdweight不为None时考虑此权重
+        if type(self.holdweight) != type(None):
+            bar_hold = [i*self.holdweight for i in bar_hold]
+        # 当period不等于1时需要按照period调整持仓
+        mat_hold = []
+        for period in self.periods:
+            # 以period为周期 调整持仓的持仓表
+            # 选取的index  period = 3  0,0,0,3,3,3,6...
+            list_take_hold = [[hold.index[int(i/period)*period]\
+                                for i in range(len(hold.index))]
+                    for hold in bar_hold]
+            list_hold = [bar_hold[i].loc[list_take_hold[i]]
+                    for i in range(len(bar_hold))]
+            # 提取的index非连续，复原到原来的连续交易日index
+            for hold in list_hold:
+                hold.index = bar_hold[0].index
+            mat_hold.append(list_hold)
+        self.mat_hold = mat_hold
+# 每个时间持仓标的数量
+    def matrix_holdn(self):
+        mat_holdn = []
+        for period_list in self.mat_hold:
+            list_holdn = [(i!=0).sum(axis=1) for i in period_list]
+            mat_holdn.append(list_holdn)
+        self.mat_holdn = mat_holdn 
+# matrix contri     每日净值对数收益率： np.log(matrix_contri[i_period][i_a_b].sum(axis=1)+1)
+    def matrix_contri(self):
+        mat_weight = []
+        mat_contri = []
+        for list_hold in self.mat_hold: 
+            # 合约市值权重  不是真实的市值 
+            list_cap = [hold * self.price for hold in list_hold]
+            list_weight = [cap.apply(lambda x: x/x.sum(), axis=1).fillna(0) for cap in list_cap]
+            # 当日收益(return*昨日weight)
+            list_contri = [(weight.shift()*self.returns).fillna(0) for weight in list_weight]
+            mat_contri.append(list_contri)
+            mat_weight.append(list_weight)
+        self.mat_contri = mat_contri
+        self.mat_weight = mat_weight
+# matrix logreturn  and returns
+    def matrix_lr(self):
+        mat_lr = []
+        mat_returns = []
+        for list_contri in self.mat_contri:
+            list_returns = [contri.sum(axis=1) for contri in list_contri]
+            list_lr = [np.log(returns+1) for returns in list_returns]
+            mat_lr.append(list_lr)
+            mat_returns.append(list_returns)
+        self.mat_lr = mat_lr
+        self.mat_returns = mat_returns
+    def matrix_turnover(self):
+        mat_turnover = []
+        # 假设当期没有换仓的权重与当期权重的差值即为换手率
+        # 换仓周期
+        for i in range(len(self.mat_weight)):
+            list_weight = self.mat_weight[i]
+            list_contri = self.mat_contri[i]
+            list_NoAdjustWeight = \
+                [list_weight[j].shift().fillna(0) + list_contri[j] for j in range(len(list_weight))]
+            list_NoAdjustWeight = [NoAdjustWeight.div(NoAdjustWeight.sum(axis=1), axis='rows') \
+                                   for NoAdjustWeight in list_NoAdjustWeight]
+            list_NoAdjustWeight = [NoAdjustWeight.fillna(0) for NoAdjustWeight in list_NoAdjustWeight]
+            list_turnover = \
+                [np.abs((list_weight[j]-list_NoAdjustWeight[j])).sum(axis=1) for j in range(len(list_weight))]
+            # 年化换手率
+            #list_turnover = [i.mean()*250 for i in list_turnover]
+            mat_turnover.append(list_turnover)
+        self.mat_turnover = mat_turnover
+    def get_result(self):
+        # 每一个period
+        for i in range(len(self.periods)):
+            #  每一个分组 每个时刻的每个分组收益率对其分组序号做回归
+            df_corr = pd.DataFrame()
+            for j in range(len(self.a_b)-1):
+                returns = pd.DataFrame(self.mat_returns[i][j])
+                returns['factor']=j
+                df_corr = pd.concat([df_corr, returns])
+            df_corr = df_corr.groupby('date').corr(method='spearman')
+            IC_series = df_corr.loc[(slice(None), 'factor'), 0]
+            # 因子指标
+            IC = IC_series.mean()
+            ICIR = IC/IC_series.std()
+            # 年化收益率和sharpe ratio
+            duryears = (self.returns.index[-1] - self.returns.index[0]).days/365
+            # 多空组合
+            LS_returns = self.mat_lr[i][-2] - self.mat_lr[i][0]
+            LS_std = LS_returns.std()*np.sqrt(250)
+            LS_return_annual = np.exp(LS_returns.sum()/duryears) - 1
+            LS_sharpe = (LS_return_annual-0.03)/LS_std
+            # 多头组合
+            L_returns = self.mat_lr[i][-2] 
+            L_std = L_returns.std()*np.sqrt(250)
+            L_return_annual = np.exp(L_returns.sum()/duryears) - 1
+            L_sharpe = (L_return_annual-0.03)/L_std
+            # 市场组合（等权）
+            M_returns = self.mat_lr[i][-1]
+            M_std = M_returns.std()*np.sqrt(250)
+            M_return_annual = np.exp(M_returns.sum()/duryears) - 1
+            M_sharpe = (M_return_annual-0.03)/M_std
+            # 多头换手率
+            turnover = self.mat_turnover[i][-2].mean()*250
+            # 考虑换手率造成的交易成本后的多头收益率
+            real_return = (L_return_annual+1)*(1-self.comm/10000)**(turnover) - 1
+            real_sharpe = (real_return-0.03)/L_std
+            record = {'group IC':IC, 'group ICIR':ICIR, 'L&S return': LS_return_annual, 
+                      'L return':L_return_annual, 'market return':M_return_annual, 
+                      'L&S sharpe':LS_sharpe, 'L sharpe':L_sharpe, 'market sharpe':M_sharpe, 
+                        'real return':real_return, 'real sharpe':real_sharpe, 'turnover':turnover}
+            self.result.loc[self.periods[i]] = record
+
 # plot
 # 因子组合收益（单边做多，考虑交易成本（默认单边万7））
-    def HoldReturn(self, i_period, dateleft=None, dateright=None, cost=0):
+    def HoldReturn(self, i_period=0, dateleft=None, dateright=None, cost=0):
         if dateleft==None:
             dateleft = self.factor.index[0][0]
         if dateright==None:
             dateright = self.factor.index[-1][0]
         plt, fig, ax = matplot()
         ax2 = ax.twinx()
         # 画图曲线颜色和透明度区分
@@ -235,18 +365,23 @@
             ax.legend(bbox_to_anchor=(0.5, -0.7), loc=8, ncol=2)
         ax.set_title('调整频率: %d 日'%self.periods[i_period])
         ax.set_ylabel('累计净值')
         ax.set_xlim(dateleft, dateright)
         #ax.set_xlabel('日期')
         ax2.set_ylabel('持有数量')
         plt.gcf().autofmt_xdate()
-        plt.savefig("HoldReturn.png")
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-HoldReturn.png',\
+                     bbox_inches='tight')
         plt.show()
 # 各组对数收益率-等权对数收益率
-    def LogCompare(self, i_period, dateleft=None, dateright=None, ifbench=True):
+    def LogCompare(self, i_period=0, dateleft=None, dateright=None, ifbench=True):
         if dateleft==None:
             dateleft = self.factor.index[0][0]
         if dateright==None:
             dateright = self.factor.index[-1][0]
         plt, fig, ax = matplot()
         if ifbench:
             benchmark = self.mat_lr[i_period][-1].cumsum()
@@ -274,34 +409,47 @@
         ax.plot(LS, c='C0', label='L&S  anu.{r:.2f}%'.format(r=factor_return))
         ax.legend()
         ax.set_title('Period: %d bar(s)'%self.periods[i_period])
         ax.set_ylabel('Cumulative Log Return')
         ax.set_xlabel('Date')
         ax.set_xlim(dateleft, dateright)
         plt.gcf().autofmt_xdate()
-        plt.savefig("LogCompare.png")
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-LogCompare.png',\
+                     bbox_inches='tight')
         plt.show()
 # 柱状图
-    def Bar(self):
+    def Bar(self, i_period=0):
         # 按年度划分收益率
-        df_returns = pd.concat(self.mat_lr[0], axis=1)\
+        df_returns = pd.concat(self.mat_lr[i_period], axis=1)\
             .rename(columns=dict(zip(range(len(self.a_b)), self.a_b)))
         df_returns['year'] = df_returns.index.year
-        df_returns = np.exp(df_returns.groupby('year').sum())-1
+        df_returns = 100*(np.exp(df_returns.groupby('year').sum())-1)
         # 作图
         plt, fig, ax = matplot()
         x = np.arange(len(df_returns))
         width = 0.08
         # 偏移量
         move = np.arange(-len(self.a_b)*width/2,len(self.a_b)*width/2,width)
         for n in range(len(self.a_b)):
             ax.bar(np.arange(len(df_returns))+move[n], df_returns[self.a_b[n]].values,\
                     width=width, label='%s'%(str(self.a_b[n])))
         ax.legend(bbox_to_anchor=(0.5,-0.3), loc=10, ncol=3)
         plt.xticks(x, list(df_returns.index), fontsize=20)
+        ax.set_ylabel("(%)")
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-Bar.png',\
+                     bbox_inches='tight')
+        plt.show()
 # 各组分组因子值阈值和数量
     def FactorThreshold(self):
         plt, fig, ax = matplot()
         # 颜色与LogCompare中相同，最大值和最小值为橙色C1
         # 等权指数不画
         number = len(self.a_b)-1
         number0 = int(number/2)
@@ -332,139 +480,22 @@
         ax.legend()
         ax.set_ylabel('Factor thershold')
         # 避免显示异常值
         ax2.set_ylabel('Factor group stock number')
         ax.set_xlabel('Date')
         ax.set_xlim(self.returns.index[0], self.returns.index[-1])
         plt.gcf().autofmt_xdate()
-        plt.savefig("FactorThreshold.png")
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
+        plt.savefig('./output/alpha-Portfolio-FactorThreshold.png',\
+                     bbox_inches='tight')
         plt.show()
-# mat[period][factor range]  list[factor range]
-# 获得每个持仓周期 每个因子区间的 hold （虚拟持仓 只保证比例关系正确, 和为1)  a_b factor range from a to b 区间内市值等权重
-    def matrix_hold(self):
-    # 每个bar按标的等权配置需要的持仓
-        factor = self.factor.reset_index()
-        # 选取因子值 满足a_b list中全部条件的 放置于list_hold (前开后闭，与Rank函数返回的(0，1]对应)
-        bar_hold = [factor[(i[0]<factor['factor']) & (factor['factor']<=i[1])] for i in self.a_b]
-        self.group_number = [i.groupby('date').count() for i in bar_hold]
-        # 在date没有出现的code补np.nan
-        bar_hold = [pd.DataFrame(i.pivot_table('factor', 'date', 'code'),\
-                                 index=self.factor.index.get_level_values(0).unique())\
-                                     for i in bar_hold]
-        # 非null的持仓数量为 1/price（持仓金额相等）
-        bar_hold = [(i.isnull().replace([True,False],[0,1])*\
-                     (1/self.price)).fillna(0) for i in bar_hold]
-        # 当holdweight不为None时考虑此权重
-        if type(self.holdweight) != type(None):
-            bar_hold = [i*self.holdweight for i in bar_hold]
-        # 按固定周期间隔选取持仓情况，向后填充
-        mat_hold = []
-        for period in self.periods:
-            # 以period为周期 调整持仓的持仓表
-            # 选取的index  period = 3  0,0,0,3,3,3,6...
-            list_take_hold = [[hold.index[int(i/period)*period] for i in range(len(hold.index))]
-                    for hold in bar_hold]
-            list_hold = [bar_hold[i].loc[list_take_hold[i]]
-                    for i in range(len(bar_hold))]
-            # 提取的index非连续，复原到原来的连续交易日index
-            for hold in list_hold:
-                hold.index = bar_hold[0].index
-            mat_hold.append(list_hold)
-        self.mat_hold = mat_hold
-# 每个时间持仓标的数量
-    def matrix_holdn(self):
-        mat_holdn = []
-        for period_list in self.mat_hold:
-            list_holdn = [(i!=0).sum(axis=1) for i in period_list]
-            mat_holdn.append(list_holdn)
-        self.mat_holdn = mat_holdn 
-# matrix contri     每日净值对数收益率： np.log(matrix_contri[i_period][i_a_b].sum(axis=1)+1)
-    def matrix_contri(self):
-        mat_weight = []
-        mat_contri = []
-        for list_hold in self.mat_hold: 
-            # 合约市值权重  不是真实的市值 
-            list_cap = [hold * self.price for hold in list_hold]
-            list_weight = [cap.apply(lambda x: x/x.sum(), axis=1).fillna(0) for cap in list_cap]
-            # 当日收益(return*昨日weight)
-            list_contri = [(weight.shift()*self.returns).fillna(0) for weight in list_weight]
-            mat_contri.append(list_contri)
-            mat_weight.append(list_weight)
-        self.mat_contri = mat_contri
-        self.mat_weight = mat_weight
-# matrix logreturn  and returns
-    def matrix_lr(self):
-        mat_lr = []
-        mat_returns = []
-        for list_contri in self.mat_contri:
-            list_returns = [contri.sum(axis=1) for contri in list_contri]
-            list_lr = [np.log(returns+1) for returns in list_returns]
-            mat_lr.append(list_lr)
-            mat_returns.append(list_returns)
-        self.mat_lr = mat_lr
-        self.mat_returns = mat_returns
-    def matrix_turnover(self):
-        mat_turnover = []
-        # 假设当期没有换仓的权重与当期权重的差值即为换手率
-        # 换仓周期
-        for i in range(len(self.mat_weight)):
-            list_weight = self.mat_weight[i]
-            list_contri = self.mat_contri[i]
-            list_NoAdjustWeight = \
-                [list_weight[j].shift().fillna(0) + list_contri[j] for j in range(len(list_weight))]
-            list_NoAdjustWeight = [NoAdjustWeight.div(NoAdjustWeight.sum(axis=1), axis='rows') \
-                                   for NoAdjustWeight in list_NoAdjustWeight]
-            list_NoAdjustWeight = [NoAdjustWeight.fillna(0) for NoAdjustWeight in list_NoAdjustWeight]
-            list_turnover = \
-                [np.abs((list_weight[j]-list_NoAdjustWeight[j])).sum(axis=1) for j in range(len(list_weight))]
-            # 年化换手率
-            #list_turnover = [i.mean()*250 for i in list_turnover]
-            mat_turnover.append(list_turnover)
-        self.mat_turnover = mat_turnover
-    def get_result(self):
-        # 每一个period
-        for i in range(len(self.periods)):
-            #  每一个分组 每个时刻的每个分组收益率对其分组序号做回归
-            df_corr = pd.DataFrame()
-            for j in range(len(self.a_b)-1):
-                returns = pd.DataFrame(self.mat_returns[i][j])
-                returns['factor']=j
-                df_corr = pd.concat([df_corr, returns])
-            df_corr = df_corr.groupby('date').corr(method='spearman')
-            IC_series = df_corr.loc[(slice(None), 'factor'), 0]
-            # 因子指标
-            IC = IC_series.mean()
-            ICIR = IC/IC_series.std()
-            # 年化收益率和sharpe ratio
-            duryears = (self.returns.index[-1] - self.returns.index[0]).days/365
-            # 多空组合
-            LS_returns = self.mat_lr[i][-2] - self.mat_lr[i][0]
-            LS_std = LS_returns.std()*np.sqrt(250)
-            LS_return_annual = np.exp(LS_returns.sum()/duryears) - 1
-            LS_sharpe = (LS_return_annual-0.03)/LS_std
-            # 多头组合
-            L_returns = self.mat_lr[i][-2] 
-            L_std = L_returns.std()*np.sqrt(250)
-            L_return_annual = np.exp(L_returns.sum()/duryears) - 1
-            L_sharpe = (L_return_annual-0.03)/L_std
-            # 市场组合（等权）
-            M_returns = self.mat_lr[i][-1]
-            M_std = M_returns.std()*np.sqrt(250)
-            M_return_annual = np.exp(M_returns.sum()/duryears) - 1
-            M_sharpe = (M_return_annual-0.03)/M_std
-            # 多头换手率
-            turnover = self.mat_turnover[i][-2].mean()*250
-            # 考虑换手率造成的交易成本后的多头收益率
-            real_return = (L_return_annual+1)*(1-self.comm/10000)**(turnover) - 1
-            real_sharpe = (real_return-0.03)/L_std
-            record = {'group IC':IC, 'group ICIR':ICIR, 'L&S return': LS_return_annual, 
-                      'L return':L_return_annual, 'market return':M_return_annual, 
-                      'L&S sharpe':LS_sharpe, 'L sharpe':L_sharpe, 'market sharpe':M_sharpe, 
-                        'real return':real_return, 'real sharpe':real_sharpe, 'turnover':turnover}
-            self.result.loc[self.periods[i]] = record
+
 
 
 # 因子分组计算
 # market, 分组变量1， 分组变量2， 分组数，取平均值变量(T日的未来收益)
 def FactorGroup(market, group_value0, group_value1=None,\
         group_value0_num=5, group_value1_num=3, returns_key='f-returns', delay=0,\
             level0s=None, level1s=None):
```

### Comparing `FreeBack-3.0.0b0/FreeBack/barbybar.py` & `FreeBack-3.0.1a0/FreeBack/barbybar.py`

 * *Files identical despite different names*

### Comparing `FreeBack-3.0.0b0/FreeBack/display.py` & `FreeBack-3.0.1a0/FreeBack/display.py`

 * *Files identical despite different names*

### Comparing `FreeBack-3.0.0b0/FreeBack/event.py` & `FreeBack-3.0.1a0/FreeBack/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import numpy as np
 from FreeBack.post import matplot
-from yaya_quant.re.my_pd import parallel_group
+from FreeBack.my_pd import parallel_group
 
 
 class Event():
     '''
     事件驱动测试
     参数格式:
     multi——index: date, code
```

### Comparing `FreeBack-3.0.0b0/FreeBack/my_pd.py` & `FreeBack-3.0.1a0/FreeBack/my_pd.py`

 * *Files identical despite different names*

### Comparing `FreeBack-3.0.0b0/FreeBack/post.py` & `FreeBack-3.0.1a0/FreeBack/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 import datetime
 import statsmodels.api as sm
 from plottable import ColumnDefinition, ColDef, Table
 from matplotlib.colors import LinearSegmentedColormap
 from FreeBack.display import *
 import os
   
-if 'output-post' in os.listdir():
-    pass
-else:
-    os.mkdir('output-post')
 
 '''
 # matplot绘图
 def matplot(r=1, c=1, sharex=False, sharey=False, w=8, d=5):
     # don't use sns style
     sns.reset_orig()
     #plot
@@ -321,18 +317,22 @@
             ax2 = ax.twinx()
             ax2.fill_between(self.drawdown.index,-100*self.drawdown, 0, color='C1', alpha=0.1)
             ax.set_ylabel('累计净值')
             ax.set_xlabel('日期')
             ax2.set_ylabel('回撤 (%)')
             ax.set_xlim(self.net.index[0], self.net.index[-1])
             plt.gcf().autofmt_xdate()
+        if 'output' in os.listdir():
+            pass
+        else:
+            os.mkdir('output')
         if type(filename) == type(None):
-            plt.savefig('./output-post/pnl.png')
+            plt.savefig('./output/pnl.png')
         else:
-            plt.savefig('./output-post/'+filename)
+            plt.savefig('./output/'+filename)
         plt.show()
 
 
 
 # 传入barbybar运行完毕的world对象
 class Post():
     # benchmark为收益率（非对数收益率）
```

### Comparing `FreeBack-3.0.0b0/LICENSE` & `FreeBack-3.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeBack-3.0.0b0/README.md` & `FreeBack-3.0.1a0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-# -----------------------FreeBack------------------------
+# -----------------------Module------------------------
 
 **barbybar**： 逐k线，逐笔成交的事件驱动回测
 
 **alpha**: 因子测试
 
 **event**：事件信号测试
 
 **post**： 后处理模块
 
 **display**： 可视化模块
 
 **my_pd**：pandas常用操作
 
 # -----------------------INSTALL-------------------------
-手动安装:     
+从pypi安装:
 
-              git clone https://github.com/LHanLi/FreeBack.git
-              
-              cd FreeBack
-              
-              python3 setup.py install --u
-              
-自动安装:
-
-            pip3 install --upgrade --user   git+https://github.com/LHanLi/FreeBack.git
+            pip install FreeBack==3.0.0b0
+从github安装： pip3 install --upgrade --user   git+https://github.com/LHanLi/FreeBack.git
+            python setup.py develop
 
 # ----------------------Hello world-----------------------
```

