package cn.demo.controller;

import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.servlet.ModelAndView;

//控制器
@Controller
public class Sj1{
	
	@RequestMapping("/sj1")
	public ModelAndView sj1() {
		System.out.println("学框架就学Spring MVC");
		ModelAndView mav=new ModelAndView("index");
		ModelAndView mav1=new ModelAndView();
		mav1.setViewName("index");
		mav.addObject("num", 123456);
		return mav;
	}
}
