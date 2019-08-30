package cn.demo.controller;

import java.util.Map;

import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestMethod;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.servlet.ModelAndView;
import org.springframework.web.servlet.mvc.AbstractController;

//控制器
/*public class IndexController extends AbstractController {

	@Override
	protected ModelAndView handleRequestInternal(HttpServletRequest arg0, HttpServletResponse arg1) throws Exception {
		// TODO Auto-generated method stub
		System.out.println("Hello,SpringMVC");
		ModelAndView mav=new ModelAndView("index");
		ModelAndView mav1=new ModelAndView();
		mav1.setViewName("index");
		return mav;
	}

}*/

//控制器
@Controller
public class IndexController{
	
	@RequestMapping("/index")
	public ModelAndView index1() {
		System.out.println("Hello,SpringMVC");
		ModelAndView mav=new ModelAndView("index");
		ModelAndView mav1=new ModelAndView();
		mav1.setViewName("index");
		mav.addObject("num", 123456);
		return mav;
	}
	
	@RequestMapping("/index2")
	public String index2(Model model,String userName) {
		model.addAttribute("num", 12345);
		System.out.println(userName);
		return "index";
	}
	
	
	@RequestMapping(value="/index3",method=RequestMethod.GET,params={"userName"})
	public String index3(String userName) {
		System.out.println(userName);
		return "index";
	}
	
	
	@RequestMapping(value="/index4",method=RequestMethod.GET)
	public String index4(@RequestParam("userName")String userName) {
		System.out.println(userName);
		return "index";
	}
	
	@RequestMapping(value="/index5",method=RequestMethod.GET)
	public String index5(@RequestParam(value="userName",required=false,defaultValue="1s")String userName) {
		System.out.println(userName);
		return "index";
	}
	
	@RequestMapping("/index6")
	public String index6(Map<String, Object> map,String userName) {
		map.put("num", 12345);
		System.out.println(userName);
		return "index";
	}
	
	
	
}
