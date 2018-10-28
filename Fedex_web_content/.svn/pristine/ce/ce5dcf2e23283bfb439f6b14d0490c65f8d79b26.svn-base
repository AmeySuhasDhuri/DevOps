package com.fedex.Loginservices;

import org.junit.Assert;
import org.junit.Test;

import com.fedex.services.LoginService;
import com.fedex.vo.LoginVo;



public class TestLoginservices {
	
	@Test
	public void testcheckLogin_ValidParams(){
	String id = "123";
	String password = "123";
	LoginVo loginVo = new LoginVo(id, password);
	LoginService loginService = new LoginService();
	boolean result = loginService.checkLogin(loginVo);
	Assert.assertTrue(result);	
	}
	
	@Test
	public void testcheckLogin_InValidPassword(){
	String id = "User";
	String password = "";
	LoginVo loginVo = new LoginVo(id, password);
	LoginService loginService = new LoginService();
	boolean result = loginService.checkLogin(loginVo);
	Assert.assertFalse(result);	
	}

	@Test
	public void testcheckLogin_InValidId(){
	String id = "";
	String password = "12345";
	LoginVo loginVo = new LoginVo(id, password);
	LoginService loginService = new LoginService();
	boolean result = loginService.checkLogin(loginVo);
	Assert.assertFalse(result);	
	}
	
	@Test
	public void testcheckLogin_noParams(){
	String id = "";
	String password = "";
	LoginVo loginVo = new LoginVo(id, password);
	LoginService loginService = new LoginService();
	boolean result = loginService.checkLogin(loginVo);
	Assert.assertTrue(result);	
	}
	
	@Test
	public void testcheckLogin_InValidParams(){
	String id = "User";
	String password = "12134";
	LoginVo loginVo = new LoginVo(id, password);
	LoginService loginService = new LoginService();
	boolean result = loginService.checkLogin(loginVo);
	Assert.assertFalse(result);	
	}
}
