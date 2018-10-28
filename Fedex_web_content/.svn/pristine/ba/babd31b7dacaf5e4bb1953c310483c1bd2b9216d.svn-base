package com.fedex.servlet;

import java.io.IOException;

import javax.servlet.RequestDispatcher;
import javax.servlet.ServletException;
import javax.servlet.http.HttpServlet;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

import com.fedex.services.LoginService;
import com.fedex.vo.LoginVo;


public class LoginServlet extends HttpServlet {

	private static final String USR_PARM_NAME = "userName";
	private static final String PASS_PARM_NAME = "password";
	private static final String INDEX_PAGE_URL = "index.html";
	private static final String LOGIN_FAILED_URL = "login.html";
	
	
	
	@Override
	protected void doPost(HttpServletRequest request, HttpServletResponse response)
			throws ServletException, IOException {

		
		String userId = request.getParameter(USR_PARM_NAME);
		String password = request.getParameter(PASS_PARM_NAME);
		LoginService loginService = new LoginService();
		LoginVo  loginVo = new LoginVo(userId, password);
		boolean result = loginService.checkLogin(loginVo);
		System.out.println("Result is : "+result);
		String url = result?INDEX_PAGE_URL:LOGIN_FAILED_URL;
		System.out.println("URL is : "+url);
		RequestDispatcher rd = request.getRequestDispatcher(url);
		rd.forward(request, response);
		
	}
	
	@Override
	protected void doGet(HttpServletRequest request, HttpServletResponse response)
			throws ServletException, IOException {

		doPost(request, response);
	}
	
}
