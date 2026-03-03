# <center><font face="楷体">薪火笔记社</center>

# 热力学基础
##### “学熵心伤，学焓心寒，学㶲心拥，学㷻心芜”  ——张亚宁
### 白口半牛
#### 2025.1.3

---

# 前言

#### 写在前面

平心而论，热力学基础并非什么很难的课程。这门课可能是人生中第一门思想大于解题的课，通过这门课程，即可瞥见专业课教育的一角：无习题、无往年题、概念抽象、分数构成一直在完善、需自发勘误......  
>“热工基础是热工技术理论的基础，是工程热力学和传热学的有机结合，是研究热能的传递、热能有效利用以及热能和机械能等其它能量转换规律及其应用的工程技术学科。课程的主要目标是使学生掌握热力学和传热学的基本规律，并能正确运用这些规律对热工过程进行分析和计算。本课程不仅为学生学习有关专业课程提供必要的基础理论知识，而且为学生毕业后从事热能利用、热设计、热管理和热控制等方面的专业技术工作和科学研究工作打下必要的理论基础。在教学过程中结合本课程特点，注意培养学生辨证思维和逻辑推理的能力；训练其建立热力学和传热学模型的能力；着重培养学生对热工问题的判断、计算和综合能力分析能力；着重培养学生的创新精神和实践能力。（1）建立起热力学的基本概念，掌握对其结构特征和工作指标的判定和设计方法，使其（2）具有完成热力系统、能源装备热力性能分析的能力，（3）自主学习和终身学习的意识，有不断学习和适应发展的能力，为他们将来在本领域的工作打下比较坚实的基础。”[^1]  
<p>从教学大纲可以看出，课程开设初心是好的，但是在实际的听课授课过程中出现了较多的不和谐的因素，尤其是在笔者所在的学院尤为明显。</p>  
<p>如果对课程进度进行合理规划，确保前后两个老师教授的内容衔接顺畅，避免出现教学内容重复或遗漏现象。且让前期授课教师关注课程本身内容，按照教学大纲进行授课，确保学生掌握热力学基础知识，尊重学生的专业选择，不宜在课堂上频繁宣传所在专业，拉踩其他专业的话，或许也就不会出现80多人挂科30多个的荒谬事件了。
</p>
<p>如果读到这篇笔记的你恰好不慎选择了这门课程，那笔者建议如果不是非要去能源学院的话抓紧退课。不要被开始的表相迷惑，以2024秋季学期为例，这是一门期末考式占80分（轻计算，重证明和概念），还有10的论文大作业（要求阅读sci、nature等后撰写），并不是可以蒙混过关的水课。那如果已经不幸的像笔者当年一样错过了退课期，便只能拨冗阅读一下这篇笔记了。</p>

---

# 目录[^2][^3]

1. [第一章：基本概念](#第一章：章节标题)
2. [第二章：热力学第一定律](#第二章：章节标题)
3. [第三章：气体的热力性质和热力过程](#第三章：章节标题)
4. [第四章：热力学第二定律](#第四章：章节标题)
5. [第五章：气体的流动和压缩](#第五章：章节标题)
6. [第六章：空气动力循环](#第六章：章节标题)
7. [第七章：水蒸气性质和蒸汽动力循环](#第七章：章节标题)
8. [第八章：制冷循环](#第八章：章节标题)
9. [第九章：湿空气性质和湿空气过程](#第九章：章节标题)

---

# 第一章：基本概念
1. **热力系**
   - 含义:人为的具体的热力学研究对象
   - 选取原则：可大可小，有边界
   - 外界：热力系之外于热力系相互作用的物体
        1.热作用源
        2.功作用源
        3.物质作用源
   - 界面：热力系于外界分界面
   - 分类：闭口系、开口系、绝热系、孤立系......
2. **状态和状态参数**
   - 状态：热力系在指定瞬间所呈现的全部宏观性质的总称
   - 状态参数：从各个不同方面描写宏观状态的物理量，其中常用的有：p、v、T、U、H、S
   - 基本状态参数：p、v、T
   >1.温度T  
   $\frac{mc^2}{2}=\frac{3}{2}kT$
   $t = T - 273.15K$


   >2.压力p
   $p = \frac{F}{A}$
   大气压：$p_b$
   绝对压力：$p$
   表压力：$p_g = p - p_b$
   真空度：$p_v = p_b - p$

   >3.比体积v
   $v = \frac{V}{m} = \frac{1}{\rho}$
   $V = mv$

   >4.焓H
   $H = U + pV$
   比焓：$h = \frac{H}{m} = u + pv$

   >5.熵S
   $S = \int\frac{du + pdv}{T} + S_0$
   $dS= \frac{dU + pdV}{T}$

   >6.热力学能U
   $\varDelta U = W + \varDelta Q$
3. **平衡状态与状态方程**
宏观性质不随时间变化，对于简单热力系，给出两个相互独立的状态参数即可确定其他。  
p、v、T为基本状态参数，状态方程是关于基本状态参数的方程。eg.$p = f(v,T)$
4. **过程与循环**
   - 过程：热力系从一个状态到另一个状态
   - 内平衡过程：从一个平衡态经过中间无数个平衡态变为另一个平衡态
   - 循环：封闭的过程
5. **功与热转换（过程量）**
   - 功W
     1.膨胀功：$w = pdv$
     2.对外做功为正，W>0；对外做功为负，W<0
   - 热量Q
     1.$Q = TdS$
     2.传热：q，吸热，q>0；放热，q<0
   - 特征：过程量，与路径有关

---


# 第二章：热力学第一定律
1. **功**
  - $w_v$膨胀功：$pdv$
  - 推动功：$pV$
  - $wt$技术功：$-vdp$（动力机械一个周期内获得的功）
2. **热力学第一定律**
   能量守恒与转换原理，否定了第一类永动机
![一般热力系能量](img\e.jpg "一般热力系能量")
   1. 一般热力系能量
     - 总能量：$E$
     - 热力系能：$U$，宏观动能$E_k$，重力位能$E_p$
     - $E = U + E_k + E_p$
     - 微分：$\delta Q = dE + (e_2\delta m_2 - e_1\delta m_1 ) + \delta W_{tot}$
     - 积分：$Q = \varDelta E + \int_{(\tau)} (e_2\delta m_2 - e_1\delta m_1) + W_{tot}$
   2. 闭口系
     >$e_2\delta m_2 = e_1\delta m_1 = 0$
     $\delta Q = dE + \delta W_{tot}$
      $\delta q = du + \delta w_{tot} = du + pdv$（无摩擦时）
   3. 开口系
   >$\delta q = dh + \delta w_t = du + p_2v_2 - p_1v_1 + \delta w_t  = du + vdp + pdv + \delta w_t$
   因为$\delta q = du + pdv$
   故有$\delta w_t = - vdp$
   4. 稳流
   流道中任意一点的状态参数都不随时间变化的流动
   >$dE = 0，\delta m_1 = \delta m_2$
   $\delta Q = (e_2\delta m_2 - e_1\delta m_1 ) + \delta W_{shaft}$（轴功）
   $\delta q = e_2 - e_1 + \delta w_{sh}$
   $e = h + \frac{1}{2}c^2 + gz$
   - 动力机：$\frac{1}{2}\varDelta c^2，g\varDelta z，q$可忽略$w_{sh} = w_t = h_1 - h_2$，即动力机做功为工质的焓降
   - 换热器：$\delta q = h_1 - h_2$
   - 节流：$c_1 \approx c_2，h_1 = h_2$，即节流前后焓不变，但不是定焓过程
3. **循环**
 $q_0 = w_0$，净热等于净功

 ---

# 第三章：气体的热力性质和热力过程
1. **理想气体与实际气体**
   - 理想气体：分子无体积、无作用力（高温低压气体可近似为理想气体）eg.空气、燃气、烟气、湿空气
   - 实际气体：分子有体积、有作用力 eg.热机蒸汽、制冷蒸汽
2. **理想气体状态方程和摩尔气体常数**
   - $pv = R_gT$
   - $R_g = \frac{R}{M}$
   >$R$:通用气体常数
   $R_g$:气体常数
3. **理想混合气体**
   - 相对成分：$\omega_i$质量分数、$x_i$摩尔分数、$\phi_i$体积分数
   - 绝对成分：$m、n、v$
   - $R_{g,mix} = \frac{R}{M_{mix}}$
   - $M_{mix} = \frac{1}{\Sigma\frac{\omega_i}{M_i}}$
   - $x_i = \frac{\frac{\omega_i}{M_i}}{\Sigma\frac{\omega_i}{M_i}}$
   - 道尔顿定律：$p_{mix} = \Sigma p_i$ $p_i = p_{mix}x_i$
4. **气体热力性质**
   >$c_V = \frac{\varDelta q_V}{dT} = \frac{du + pdv}{dT} = \frac{du}{dT}$
   $c_p = \frac{\varDelta q_p}{dT} = \frac{dh - vdp}{dT} = \frac{dh}{dT} = \frac{d(u + pv)}{dT} = \frac{du + R_gdT}{dT} = c_V + R_g$
   $$
   \begin{cases}
    du = c_VdT \\
    dh = c_pdT
   \end{cases}
   \begin{cases}
    \gamma=\frac{c_p}{c_V} \\
    c_p - c_V = R_g
   \end{cases}
   \begin{cases}
    c_V = \frac{R_g}{\gamma - 1} \\
    c_p = \frac{\gamma R_g}{\gamma - 1}
   \end{cases}
   $$
   $ds = \frac{du + pdv}{T} = \frac{c_VdT}{T} + \frac{R_gdv}{v} =\frac{dh - vdp}{T} = \frac{c_pdT}{T} - \frac{R_gdp}{p}$
   - 定容：$s = c_VlnT + R_glnv + C_1$ $T = e^{\frac{s - C_1'}{c_V}}$
   - 定压：$s = c_plnT - R_glnp + C_2$ $T = e^{\frac{s - C_2'}{c_p}}$
5. **经典热力过程**
![p-v](img\pv.png "p-v")

![p-v](img\ts.png "T-s")
   - 定容：$w_V=pdv=0$ $w_t=v(p_1-p_2)$ $q_V=u_2-u_1=c_V(T_2-T_1)$
   - 定压：$w_p=p(v_2-v_1)$ $w_{t,p}=-vdp=0$ $q_p=h_2-h_1=c_p(T_2-T_1)$
   - 定温：$w_T=\int pdv=R_gTln\frac{v_2}{v_1} = w_{t,T}=-\int vdp=R_gTln\frac{p_1}{p_2}=q_T$
   - 定熵：$ds=\frac{du+pdv}{T}=0$
     >$\delta q = du + \delta w = c_VdT+pdv → c_VdT=-pdv① $
      $\delta q = dh + \delta w_t = c_pdT-vdp → c_pdT=-vdp② $
      $\frac{②}{①} = \frac{c_pdT}{c_VdT}=\gamma=\frac{vdp}{-pdv} → pv^{\gamma}=C$
      $w_s=\int_{1}^{2}pdv=\int_{1}^{2}\frac{p_1v_1^\gamma}{v^\gamma}=\frac{1}{1-\gamma}(p_2v_2-p_1v_1)=\frac{R_gT_1}{\gamma - 1}[1-(\frac{p_2}{p_1})^{\frac{\gamma - 1}{\gamma}}]=\frac{p_1v_1}{\gamma - 1}[1-(\frac{p_2}{p_1})^{\frac{\gamma - 1}{\gamma}}]$
      $d(pv^{\gamma}=0) →v^\gamma dp+\gamma pv^{\gamma - 1}dv=0 → -vdp=\gamma pdv$
      $w_{t,s}=-vdp=\gamma pdv = \gamma w_s =\frac{\gamma p_1v_1}{\gamma - 1}[1-(\frac{p_2}{p_1})^{\frac{\gamma - 1}{\gamma}}]$
   - 多方：$pv^n=C$ 注：要求画图时，一定要先画出定容、定压、定温、定熵过程进行定位，再根据n的值进行绘制。
![多方过程p-v](img\npv.jpg "多方过程p-v")
![多方过程T-s](img\nTs.jpg "多方过程T-s")
---
# 第四章：热力学第二定律
1. **热力学第二定律的任务**
   描述过程的方向、限度、条件。
2. **可逆不可逆过程**
   - 可逆过程：传热无温差，运动无摩擦、内平衡
   - 不可逆过程：传热有温差，运动有摩擦 
3. **状态参数熵**
   $ds=\frac{du+pdv}{T}=\frac{du+w}{T}+\frac{Q^g}{T}$ 
4. **熵方程**
![热力系熵](img\s.jpg "热力系熵") 
   - 熵产：$S_g=\frac{Q^g}{T}≥0$
   - 热熵流：$S_f=\frac{Q}{T}$
   - 质熵流：$ms$
   - 一般：$dS=(s_1\delta m_1-s_2\delta m_2)+\delta S_f+\delta S_g$
   - 闭口：$dS = \delta S_f + \delta S_g$
   - 绝热：$dS = (s_1\delta m_1-s_2\delta m_2) + \delta S_g$
   - 绝热闭口：$dS=S_g$
   - 孤立系熵增原理：$\varDelta S_{iso}=S_g≥0$
5. **各种表述的等效性**
   - Clausius:不可能将热从低温物体传至高温物体而不引起其它变化
   >反证法：$T_L < T_H $ $\varDelta S_{iso}=-\frac{Q}{T_L}+\frac{Q}{T_H}<0$ 由孤立系熵增原理，矛盾
   - Kelvin·Planck:不可能从单一热源吸取热量使之完全变为有用功而不产生其他影响
   >反证法：$\varDelta S_{iso}=-\frac{Q}{T}+0<0$ 由孤立系熵增原理，矛盾
6. **Carnot循环和定理**
   - Carnot循环:卡诺循环包括四个步骤：等温吸热，在这个过程中系统从高温热源中吸收热量；定熵膨胀，在这个过程中系统对环境作功，温度降低；等温放热，在这个过程中系统向环境中放出热量，体积压缩；定熵压缩，系统恢复原来状态，在等温压缩和绝热压缩过程中系统对环境作负功。卡诺循环可以想象为是工作于两个恒温热源之间的准静态过程，其高温热源的温度为$T_H$，低温热源的温度为$T_L$
   - $\eta_c = 1 - \frac{T_L}{T_H}$
![Carnot循环](img\Carnot.jpg "Carnot循环") 
   - Carnot定理：$\eta_{th}≤\eta_c$
     > $\eta_{th}=\frac{W}{Q_1}$ $W = Q_1-Q_2$
     $\varDelta S_{iso}=-\frac{Q_1}{T_H} + \frac{Q_2}{T_L}≥0$
     $\frac{Q_2}{T_L}≥\frac{Q_1}{T_H}$
     $\frac{Q_1-W}{T_L}≥\frac{Q_1}{T_H}$
     $\frac{Q_1-W}{Q_1}≥\frac{T_L}{T_H}$
     $\eta_{th}≤\eta_c= 1 - \frac{T_L}{T_H}$
7. **Clausius分式**
   - $\oint \frac{\delta Q}{T}≤0$
   - $\varDelta S_{1-2} = S_2 - S_1≥\int_{1}^{2}\frac{\delta Q}{T}$
   - 当且仅当可逆时取等


---


# 第五章：气体的流动和压缩
1. **一元稳定流动**
   - 概念：所谓一元流动，是指流动的一切参数仅沿一个方向(这个方向可以是直线，也可以是弯曲流道的轴线)有显著变化，而在其他两个方向上的变化是很小的。所谓稳定流动，是指流道中任意指定空间的一切参数都不随时间而变化。
   - 质量方程：$\frac{Ac}{v}=C$（连续性方程）
     >$v=\frac{V}{m}=\frac{1}{\rho}$
     $q_m=\frac{m}{t}=\frac{\rho V}{t}=\frac{\rho Act}{t}=\rho Ac=\frac{Ac}{v}=C$
   - 能量方程：$h + \frac{1}{2}c^2=C$
     >$\delta Q = dE + (e_2\delta m_2 - e_1\delta m_1 ) + \delta W_{shaft}$
     $\delta Q=0$ $ dE=0$ $m_1=m_2$ $ \delta W_{shaft}=0 → e_1=e_2=C$
     $e = h + \frac{1}{2}c^2 +gz$ $z=0$
   - 动量方程：$-vdp-\frac{v}{A}dF_f=cdc$
![动量方程](img\p.jpg "动量方程") 
     >$Fdt=dmdc$
     $[p-(p+dp)]A-dF_f=\frac{dmdc}{dt}$
     $-dp-\frac{dF_f}{A}=\frac{dmdc}{Adt}$
     $-dp-\frac{dF_f}{A}=\frac{Adxdc}{vAdt}$
     $-vdp-\frac{v}{A}dF_f=cdc$
   - 状态方程：$pv=R_gT$
   - 过程方程：$pv^{\gamma}=C$
   - 声速方程：$c_s=\sqrt{\gamma pv}=\sqrt{\gamma R_gT}$
2. **喷管**
   - 概念：利用压力降落而使流体加速的管道
     >$\frac{Ac}{v}=C → \frac{dA}{A}+\frac{dc}{c}-\frac{dv}{v}=0$（取对数）
     $h + \frac{1}{2}c^2=C → cdc=-vdp$ （求导）
     $pv^k=C →  \frac{dp}{p}=-\frac{kdv}{v}$（$k$为定熵系数，对于定比热容理想气体，$k=\gamma_0$）
     $Ma=\frac{c}{c_s}$（马赫数）
     $\frac{dA}{A}+\frac{dc}{c}+\frac{dp}{kp}=0$
     $\frac{dA}{A}+\frac{dc}{c}+\frac{vdp}{kvp}=\frac{dA}{A}+\frac{dc}{c}-\frac{cdc}{kpv}=0$
     $\frac{dA}{A}+\frac{dc}{c}-\frac{c^2dc}{c_s^2c}=0$
     $\frac{dA}{A}=(\frac{c^2}{c_s^2}-1)\frac{dc}{c}=(Ma^2-1)\frac{dc}{c}$
   - 不可压：$\frac{dA}{A}=-\frac{dc}{c}<0$ 渐缩喷管
   - 可压：$\frac{dA}{A}=(Ma^2-1)\frac{dc}{c}$
     1. $0<Ma<1$ 渐缩喷管
     2. $Ma<1 → Ma>1$ 缩放喷管（拉瓦尔喷管）
     3. $Ma>1$ 渐放喷管
3. **喷管流量**
   >$-vdp=cdc$
   $w_t=\frac{1}{2}c^2=\frac{kp_1v_1}{k-1}[1-(\frac{p_2}{p_1})^{\frac{k-1}{k}}]$
   $c=\sqrt{\frac{2kp_1v_1}{k-1}[1-(\frac{p_2}{p_1})^{\frac{k-1}{k}}]}=c_s\sqrt{\frac{2}{k-1}[1-(\frac{p_2}{p_1})^{\frac{k-1}{k}}]}$
4. **背压**
   较为复杂，且并非重点，感兴趣的读者可移至： https://b23.tv/hZOJzhn 自学
5. **压气机**
   压气方法：定温、多变、定熵
![压气机](img\air.jpg "压气机")
   耗功：$w_T<w_n<w_S$    

 ---

# 第六章：空气动力循环
1. **活塞式内燃机混合加热循环**
   - 实际情况
![实际情况](img\engine_th.jpg "实际情况")
   - 理想情况
![理想情况](img\engine.jpg "理想情况")  
     - 1-2：定熵压缩：压缩比：$\epsilon =\frac{v_1}{v_2}$
     - 2-3：定容燃烧：压升比：$\lambda = \frac{p_3}{p_2}$
     - 3-4：定压燃烧：预胀比：$\rho = \frac{v_4}{v_3}$
     - 4-5：定熵膨胀
     - 5-1：定容冷却
   >如果状态1、$\epsilon$、$\lambda$、$\rho$ 已知，则循环确定：（2024秋压轴题）
   $\eta_t = 1 - \frac{q_2}{q_1}=1-\frac{q_2}{q_{1V}+q_{1p}}$
   $q_2=c_V(T_5-T_1)$
   $q_{1V}=c_V(T_3-T_2)$
   $q_{1p}=c_p(T_4-T_3)$
   $\eta_t=1-\frac{T_5-T_1}{T_3-T_2+\gamma (T_4-T_3)}$
   $T_2=T_1(\frac{v_1}{v_2})^{\gamma - 1}=T_1\epsilon^{\gamma - 1}$
   $T_3=T_2\frac{p_3}{p_2}=T_1\epsilon^{\gamma - 1}\lambda$
   $T_4=T_3\frac{v_4}{v_3}=T_1\epsilon^{\gamma - 1}\lambda \rho$
   $T_5=T_4(\frac{v_4}{v_5})^{\gamma - 1}=T_4(\frac{v_3\rho}{v_1})^{\gamma - 1}=T_4(\frac{v_2\rho}{v_1})^{\gamma - 1}=T_1\epsilon^{\gamma - 1}\lambda \rho (\frac{\rho}{\epsilon})^{\gamma - 1}=T_1\lambda \rho^{\gamma}$
   代入得：$\eta_t =1-\frac{1}{\epsilon^{\gamma - 1}}\frac{\lambda \rho^{\gamma}-1}{(\lambda - 1)+\gamma \lambda (\rho - 1)}$
2. **定容加热循环与定压加热循环**
   - Otto循环（汽油机）
![Otto循环](img\Otto.jpg "Otto循环") 
     >$\rho = 1$
     $\eta_{t,V}=1-\frac{1}{\epsilon^{\gamma - 1}}$
   - Disel循环（柴油机）
![Disel循环](img\Disel.jpg "Disel循环")
     >$\lambda = 1$
     压增比：$\pi = \frac{p_2}{p_1}$
     $\eta_{t,p}=1-\frac{1}{\epsilon^{\gamma - 1}}\frac{\rho^{\gamma}-1}{\gamma(\rho - 1)}=1-\frac{1}{\pi \frac{\gamma - 1}{\gamma}}$ 
3. **效率比较**
   - 进气状态、压缩比、吸热相同时
![进气状态、压缩比、吸热相同时](img\Q.jpg "进气状态、压缩比、吸热相同时")
     >$\delta Q=TdS$
     $\eta = 1-\frac{q_{吸}}{q_{放}}$
     Otto:1-2-3-4'-5'-1
     Disel:1-2-4"-5"-5-1
     $q_{吸Otto}=q_{吸Disel}$
     $q_{放Otto}<q_{放Disel}$
     $\eta_{Otto}>\eta_{Disel}$
   - 进气状态、$T_{max}$、$p_{max}$相同时
![进气状态、Tmax、pmax相同时](img\Tp.jpg "进气状态、Tmax、pmax相同时")
     >$\delta Q=TdS$
     $\eta = 1-\frac{q_{吸}}{q_{放}}$
     Otto:1-2'-4-5-1
     Disel:1-2"-4-5-1
     混合：1-2-3-4-5-1
     $q_{吸Otto}=q_{吸Disel}$
     $q_{放Otto}>q_{放Disel}$
     $\eta_{Otto}<\eta_{混}<\eta_{Disel}$
4. **燃气轮机**
![燃气轮机](img\gasturbine.jpg "燃气轮机")
 ---
# 第七章：水蒸气性质和蒸汽动力循环
1. 水蒸气的饱和状态：气压最大22.64atm，373.99℃
![p-v](img\vapor_pv.jpg "p-v")
![T-s](img\vapor_ts.jpg "T-s")
![h-s](img\vapor_hs.jpg "h-s")
2. **Rankine循环**
   - 基本过程
![Rankine循环](img\Rankine.jpg "Rankine循环")
   - 效率比较
     - 提高新气温度
     ![提高新气温度](img\RankineT.jpg "提高新气温度")
     >$T_1$升高
     $\eta = 1-\frac{q_2}{q_1}\approx1-\frac{T_L}{T_H}$
     平均吸热温度$T_H$，$\eta$升高
     - 新气温度不变，提高$p_1$升高
     ![提高p1](img\RankineP.jpg "提高p1")
     >$p_1$升高
     $\eta = 1-\frac{q_2}{q_1}\approx1-\frac{T_L}{T_H}$
     平均吸热温度$T_H$，$\eta$升高
---


# 第八章：制冷循环
1. **逆Carnot循环**
![逆Carnot循环](img\antiCarnot.jpg "逆Carnot循环")
   >$q_1=w_0+q_2$
   制冷系数：$\epsilon_c = cop = \frac{q_2}{w_0}$
   $\epsilon_c = \frac{q_2}{w_0} =\frac{T_Rds}{(T_0-T_R)ds}=\frac{T_R}{T_0-T_R}=\frac{1}{\frac{T_0}{T_R}-1}$
   $\epsilon_c>1$普冷
   $\epsilon_c<1$深冷
1. **供热循环**
![供热循环](img\heat.jpg "供热循环")
   >$\zeta_c = \frac{q_1}{w_o}=\frac{T_Hds}{(T_H-T_0)ds}=\frac{T_H}{T_H-T_0}=\frac{1}{1-\frac{T_0}{T_H}}>1$

---

# 第九章：湿空气性质和湿空气过程
1. **湿空气**
   $p = p_V+p_{DA}$
   $p_V$：水蒸气分压力
   $p_{DA}$：干空气分压力
2. **湿度**
  - 绝对湿度：1$m^3$湿空气中水蒸气质量
    - 未饱和：$\rho_V = \frac{m_V}{V}=\frac{1}{v_V}$
    - 饱和：$\rho_{SV}=\frac{1}{v_{SV}}=\frac{1}{v^{\prime\prime}}$
  - 相对湿度：
    - $\phi=\frac{\rho_V}{\rho_{V,max}}=\frac{\rho_V}{\rho_{SV}}$
    - $\rho_V=\frac{p_V}{R_{g,V}T}$ $\rho_{SV}=\frac{p_{SV}}{R_{g,SV}T}$
    - $\phi=\frac{p_V}{p_{V,max}}=\frac{p_V}{p}$
---
# 后记
![98](img\98.jpg "98")
<p>写到这里，反而没什么想说的了，希望这篇笔记能起到作用，祝读者考得比笔者高吧。</p>

---

### 参考文献 
[^1]:章思龙，秦江.热工基础（48学时）-教学大纲-定稿审核版.哈尔滨工业大学
[^2]:童钧耕，王平阳，叶强.热工基础（第三版）.上海交通大学出版社，2016，ISBN：978-7-313-15136-0
[^3]:严家鵦，王永青，张亚宁.工程热力学（第六版）.高等教育出版社，2021.9，ISBN：978-7-04-056744-1
 