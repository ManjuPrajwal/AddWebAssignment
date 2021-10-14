# AddWebAssignment

Step 1. Create Database Name Called 'AddWeb' and create the table script as mentioned below
------------------------------------------------------------------------------------------------------
USE [AddWeb]
GO

/****** Object:  Table [dbo].[User]    Script Date: 10/13/2021 10:07:55 PM ******/
SET ANSI_NULLS ON
GO

SET QUOTED_IDENTIFIER ON
GO

CREATE TABLE [dbo].[User](
	[Id] [int] IDENTITY(1,1) NOT NULL,
	[FirstName] [nvarchar](max) NULL,
	[LastName] [nvarchar](max) NULL,
	[EmailID] [nvarchar](max) NULL,
	[Address] [nvarchar](max) NULL,
	[DOB] [datetime] NULL,
 CONSTRAINT [PK_User] PRIMARY KEY CLUSTERED 
(
	[Id] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]
GO

------------------------------------------------------------------------------------------------------
