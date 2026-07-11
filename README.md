1. 圓形掃描校正
公式說明：修正後的週期與頻率對應關係。

	Rate: 相機掃描頻率 (Hz)
	Period: 掃描週期 (μs)
	Round: 真圓度係數 (用於修正掃描時間)
	Res: 影像精度 (每一像素代表的實際長度)
	公式：
	Period_calc=1,000,000/Rate
	Period_final=Period×Round
	Rate_final=1,000,000/Period_final
	Speed=Rate_final×Res
	Acceleration=Speed×10
	
2. Sensor Size (um 換算)
公式說明：像素尺寸與感測器實體尺寸之換算。

	Res: 總解析度 (pixels)
	Pix: 像素尺寸 (μm)
	S: 感測器尺寸 (mm)
	公式：
	S=(Res×Pix)/1,000
	Res=(S×1,000)/Pix
	
3. 影像精度
公式說明：計算視野與像素解析度間的關係。

	FOV: 視場範圍 (mm)
	Res: 總解析度 (pixels)
	Prec: 影像精度 (mm/pixel)
	公式：
	Prec=FOV/Res
	FOV=Prec×Res
	
4. CCTV FOV 計算
公式說明：基於光學成像公式計算視野。

	FOV: 視場範圍 (mm)
	WD: 工作距離 (mm)
	SS: 感測器尺寸 (mm)
	f: 鏡頭焦距 (mm)
	公式：
	FOV=(SS×WD)/f
	SS=(FOV×f)/WD
	
5. Telecentric 計算
公式說明：遠心鏡頭常見的倍率匹配參數。

	SS: 感測器尺寸 (mm)
	m: 鏡頭倍率
	FOV: 視場範圍 (mm)
	px: 像素尺寸 (μm)
	prec: 精度 (μm/pixel)
	res: 總解析度 (pixels)
	公式：
	FOV=SS/m
	prec=px/m
	px=(SS×1,000)/res
