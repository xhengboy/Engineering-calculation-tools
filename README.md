1. 圓形掃描校正		公式說明：修正後的週期與頻率對應關係。

Line Rate: 相機掃描頻率 (Hz)

Line Period: 掃描週期 (μs)

Round: 真圓度係數 (用於修正掃描時間)

Res: 影像精度 (每一像素代表的實際長度)

公式：

1,000,000 / Line Rate = Line Period 

Line  Period × Round = Line Period final

1,000,000 / Line Period final = Rate final

Rate final × Res = Speed

Speed × 10 = Acceleration

2. Sensor Size (um 換算)	公式說明：像素尺寸與感測器實體尺寸之換算。

1mm = 1000um

Res: 總解析度 (pixels)

Pix: 像素尺寸 (μm)

S: 感測器尺寸 (mm)

公式：

( Res × Pix ) / 1,000 = S

( S × 1,000 ) / Pix = Res

3. 影像精度		公式說明：計算視野與像素解析度間的關係。

FOV: 視場範圍 (mm)

Res: 總解析度 (pixels)

Prec: 影像精度 (mm/pixel)

公式：

FOV / Res = Prec

Prec × Res = FOV

4. CCTV FOV 計算		公式說明：基於光學成像公式計算視野。

FOV: 視場範圍 (mm)

WD: 工作距離 (mm)

SS: 感測器尺寸 (mm)

f: 鏡頭焦距 (mm)

公式：

( SS × WD ) / f = FOV

( FOV × f ) / WD = SS

5. Telecentric 計算	公式說明：遠心鏡頭常見的倍率匹配參數。

SS: 感測器尺寸 (mm)

m: 鏡頭倍率

FOV: 視場範圍 (mm)

px: 像素尺寸 (μm)

prec: 精度 (μm/pixel)

res: 總解析度 (pixels)

公式：

SS / m = FOV

px / m = prec

( SS × 1,000 ) / res = px 

以上若有乘  1000  是要換算單位
